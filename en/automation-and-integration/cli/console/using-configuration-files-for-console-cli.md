---
title: Configuration files for console commands
description: Using Configuration files for Console Commands
published: true
date: 2025-07-02T16:28:41.336Z
tags: 
editor: markdown
dateCreated: 2025-07-02T16:28:38.835Z
---

# Configuration files for console commands

!!! warning "Please create a complete backup before making any changes to an interface/import. If the result is not satisfying, it can then be restored"

If you use a configuration file, you can specify the options for the console command directly.
You can then save these newly created files under /i-doit/src/handler/config/ for example.

This saves you from typing the password in plain text. into the console.
The [Console Command](commands-and-options.md) uses .ini files. The configuration file is used with `--config /path/to/config.ini or with -c /path/to/config.ini`

## The structure of the .ini

```ini
[commandArguments]
```

Currently none available.

```ini
[commandOptions]
user=admin
password=pass
tenantId=1
```

Here you can add the options of the Console Command. These options must be written in the "long form".
For more options see [Optionen und Parameter der Console](commands-and-options.md).

```ini
[additional]
```

Special parameters are entered below.
At the moment these are available for the [ldapServerId](../../../user-authentication-and-management/ldap-directory/index.md) and for [import-syslog](commands-and-options.md#import-syslog).

* * *

## Example for the command [search-index](commands-and-options.md#search-index)

First the .ini file has to be created.
We use here additionally [update](commands-and-options.md#search-index) to overwrite and create the search index.
Additionally we use [quiet](commands-and-options.md#search-index) to shorten the output and save some memory, which can be used for indexing.

```ini title="search-index.ini"
[commandArguments]
[commandOptions]
user=admin
password=pass
tenantId=1
update
quiet
[additional]
```

To use the configuration we execute the console command and specify the path to the configuration file with `--config` or `-c`.

```shell
sudo -u www-data php console.php search-index -c /var/www/html/i-doit/src/handler/config/examples/search-index.ini
```

[example-search_index.ini :material-file-download:](../../../assets/images/en/automation-and-integration/cli/console/example-search_index.ini){ .md-button .md-button--primary }

* * *

## Example for the command [notifications-send](commands-and-options.md#notifications-send)

There are no further options for this command so we only need the following options [user](commands-and-options.md#notifications-send), [password](commands-and-options.md#notifications-send).

```ini title="notifications-send.ini"
[commandArguments]
[commandOptions]
user=admin
password=pass
tenantId=1
[additional]
```

To use the configuration file we execute the console command and specify the path to the configuration file with `--config` or short with `-c`.

```shell
sudo -u www-data php console.php notifications-send -c /var/www/html/i-doit/src/handler/config/examples/notifications-send.ini
```

[example-notifications-send.ini :material-file-download:](../../../assets/images/en/automation-and-integration/cli/console/example-notifications-send.ini){ .md-button .md-button--primary }

* * *

## Example for the command [ldap-sync](commands-and-options.md#ldap-sync)

This command offers the following additional options: [ldapServerId](commands-and-options.md#ldap-sync) and [dumpConfig](commands-and-options.md#ldap-sync).
The [ldapServerId](commands-and-options.md#ldap-sync) option specifies the ldap server to use. Here the ID of the entry must be specified.
With [dumpConfig](commands-and-options.md#ldap-sync) no synchronization is executed! Only the configuration is output. Should therefore only be used for debugging.

```ini title="ldap-sync.ini"
[commandArguments]
[commandOptions]
user=admin
password=pass
tenantId=1
[additional]
import_rooms=false
defaultCompany=""
deletedUsersBehaviour=disable_login
disabledUsersBehaviour=disable_login
; LDAP Attributes are individual. This default configuration is prepared for Active Directory:
attributes[department]=department
attributes[phone_company]=telephoneNumber
attributes[phone_home]=homephone
attributes[phone_mobile]=mobile
attributes[fax]=facsimileTelephoneNumber
attributes[description]=info
attributes[personnel_number]=initials
attributes[organization]=company
attributes[location]=physicalDeliveryOfficeName
attributes[salutation]=title
attributes[street]=streetAddress
attributes[city]=l
attributes[zip_code]=postalCode
attributes[function]=title
attributes[service_designation]=title
attributes[pager]=pager
;Kategorieerweiterung Personen
attributes[custom_1]=objectSid
attributes[custom_2]=sn
attributes[custom_3]=homePhone
attributes[custom_4]=mobile
attributes[custom_5]=info
attributes[custom_6]=manager
attributes[custom_7]=company
attributes[custom_8]=department
autoReactivateUsers=false
ignoreUsersWithAttributes[]="sn"
ignoreUsersWithAttributes[]="givenName"
ignoreFunction=empty
syncEmptyAttributes=true
```

[example-ldap.ini :material-file-download:](../../../assets/images/en/automation-and-integration/cli/console/example-ldap.ini){ .md-button .md-button--primary }

To use the configuration file we execute the console command and specify the path to the configuration file with `--config` or short with `-c`.

```shell
sudo -u www-data php console.php ldap-sync -c /var/www/html/i-doit/src/handler/config/examples/ldap-sync.ini
```

List of command options and a short explanation

| Key                            | Value                                   | Description                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| ------------------------------ | --------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| import\_rooms=                 | true or false                           | Imports the LDAP attribute physicalDeliveryOfficeName and creates it as room, without location, if not available                                                                                                                                                                                                                                                                                                                                                                               |
| defaultCompany=""              | "Name of Organisation"                  | Default Organization to be entered, leave empty if nothing should be changed                                                                                                                                                                                                                                                                                                                                                                                                                   |
| deletedUsersBehaviour=         | archive, delete or disable\_login       | Behavior for deleted LDAP users. Should these be archived, deleted or the login deactivated                                                                                                                                                                                                                                                                                                                                                                                                    |
| disabledUsersBehaviour=        | archive, delete or disable\_login       | Behavior for disabled LDAP users. Should these be archived, deleted or the login deactivated                                                                                                                                                                                                                                                                                                                                                                                                   |
| rooms\[\]=""                   | \["Room 01"\]="userPrincipalName"       | Here your room is statically assigned to an LDAP user                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| attributes\[\]=                | attributes\[i-doit field\]=AD Attribute | Possible i-doit fields: academic\_degree, function, service\_designation, street, city, zip\_code, phone\_company, phone\_home, phone\_mobile, fax, pager, personnel\_number, department, company, office, ldap\_id, ldap\_dn, description. If user-defined information is to be stored here, the [Category extension](../../../system-administration/administration/import-and-interfaces/ldap/attribute-extension.md) can be activated. Then the fields: custom\_1 - custom\_8 are available |
| autoReactivateUsers=           | true or false                           | All users are automatically set to normal status before they are synced. This function is only necessary for OpenLDAP and NDS, because it is always enabled in the Active Directory                                                                                                                                                                                                                                                                                                            |
| ignoreUsersWithAttributes\[\]= | ignoreUsersWithAttributes\[\]="sn"      | Disables the synchronization of users where e.g. the sn(Last Name) in AD is empty. Several AD attributes can be used here, see example                                                                                                                                                                                                                                                                                                                                                         |
| ignoreFunction=                | empty\*, !empty, isset\*, !isset        | The check function for "ignoreUsersWithAttributes". If the value is set to "empty", the function checks if the specified "ignoreUsersWithAttributes" value is empty. If this is the case the user will not be synchronized.                                                                                                                                                                                                                                                                    |

\*empty - Checks if a variable contains a value
\*isset - Checks if a variable exists and if it is not NULL

* * *

## Example for the command [import-syslog](commands-and-options.md#import-syslog)

There are no further options for this command so we only need the following options [user](commands-and-options.md#import-syslog), [password](commands-and-options.md#import-syslog) und [tenantId](commands-and-options.md#import-syslog).

```ini title="import-syslog.ini"
[commandArguments]
[commandOptions]
user=admin
password=admin
tenantId=1
[additional]
; splits syslog-line in several parts
; "/(^[a-zA-Z]{3}[ ]+[\d]+ [\d\:\d]+) " .  /* date / time */
; "(([.\-0-9a-zA-Z]+)*" .                  /* hostname */
; "(\b(?:\d{1,3}\.){3}\d{1,3}\b)*)+ " .    /* IP-Address */
; "([a-zA-Z0-9-_\/\[\]:]+) " .             /* Process name */
; "(.*)/";                                 /* Syslog-Message */
regexSplitSyslogLine="/(^[a-zA-Z]{3}[ ]+[\d]+ [\d\:\d]+) (([.\-0-9a-zA-Z]+)*(\b(?:\d{1,3}\.){3}\d{1,3}\b)*)+ ([a-zA-Z0-9-_\/\[\]:]+) (.*)/";
priorities[]=Emergency
priorities[]=Alert
priorities[]=Critical
priorities[]=Error
priorities[]=Warning
priorities[]=Notice
priorities[]=Info
priorities[]=Debug
logfiles[]="/var/log/system.log"
alertlevels[] = 4
alertlevels[] = 4
alertlevels[] = 3
alertlevels[] = 3
alertlevels[] = 2
alertlevels[] = 2
alertlevels[] = 1
alertlevels[] = 1
```
