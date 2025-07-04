---
title: Settings for [Tenant name]
description: Settings for [Tenant name]
published: true
date: 2025-07-02T16:32:24.034Z
tags: 
editor: markdown
dateCreated: 2025-07-02T16:32:21.579Z
---

# Settings for [Tenant name]

Here you will find tenant related settings. All settings can be expanded using `Expand all` and collapsed again using `Collapse all`.

[![overview](../../../assets/images/en/system-administration/administration/tenant-mangement/settings/overview.png)](../../../assets/images/en/system-administration/administration/tenant-mangement/settings/overview.png)

## Password reset option

| Option                | Value                                |
| --------------------- | ------------------------------------ |
| Password reset option | Activated or disabled for the tenant |

## URL Settings

| Option               | Value         |
| -------------------- | ------------- |
| i-doit address (URL) | URL to i-doit |

## CMDB

| Option                                                          | Value                                                                                             |
| --------------------------------------------------------------- | ------------------------------------------------------------------------------------------------- |
| CSV-export delimiter                                            | Comma, Semicolon, Hash or Tab                                                                     |
| One-Click-Edit                                                  | Yes or No                                                                                         |
| Global SYS-ID Prefix                                            | String                                                                                            |
| Change Cable's CMDB status into 'In Operation' after attaching  | Yes or No                                                                                         |
| Change Cable's CMDB status into 'Inoperative' after detaching   | Yes or No                                                                                         |
| Object type constant for rack segment objects                   | String                                                                                            |
| Order of vertical rack slots                                    | Standard<br>From top left to bottom right, both sides<br>From top left to bottom right, each side |
| Mirror the rear vertical rack slots                             | Yes or No                                                                                         |
| Displaying multiple RUs                                         | From top<br>From bottom                                                                           |
| Detached segment objects...                                     | should remain unchanged<br>should be archived<br>should be purged                                 |
| Detach objects when relocating from a chassis                   | Yes or No                                                                                         |
| Activate Interaction between "Logical location" and "Location"? | Yes or No                                                                                         |
| Activate object type filter on workstations?                    | Yes or No                                                                                         |
| Remove object IDs from CSV exported lists.                      | Yes or No                                                                                         |
| Disable MAC address validation                                  | Yes or No                                                                                         |
| SYS-ID read only                                                | Yes or No                                                                                         |
| Releasing of ip-addresses when object gets archived or deleted  | Yes or No                                                                                         |
| Keep status of imported objects?                                | Yes or No                                                                                         |
| Prefix for auto-naming of cable objects                         | Empty or String                                                                                   |
| Activate quickpurge button                                      | Yes or No                                                                                         |
| WYSIWYG editor in categories                                    | Yes or No                                                                                         |
| Activate all WYSIWYG editor functions                           | Yes or No                                                                                         |
| Save my-doit CMDB-Status selection                              | Yes or No                                                                                         |

## Display Limits

| Option                                                  | Value                      |
| ------------------------------------------------------- | -------------------------- |
| Display limit for object browser objects                | Value                      |
| Display style for object browser objects                | Comma separated<br>As list |
| Amount of preloaded pages in report lists               | Value                      |
| Display limit of multi value category fields            | Value                      |
| Object-Browser result limit                             | Value                      |
| Display limit of VLANs in port lists                    | Value                      |
| Display limit of Layer-2 networks in port lists         | Value                      |
| Only show default VLAN in port overview                 | Yes or No                  |
| Display limit of assigned connectors in connector lists | Value                      |
| Display limit of Host Addresses                         | Value                      |
| Display limit of services in the CMDB explorer popup    | Value                      |
| Depth limit of the location path                        | Value                      |
| MyDoIt task entries                                     | Value                      |

## Options for the IP-List
<!-- cSpell:disable -->
| Option                      | Value                                                                                                                                                                            |
| --------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Cache lifetime (in seconds) | Value                                                                                                                                                                            |
| Ping function               | Ping via NMAP<br>Ping via FPING                                                                                                                                                  |
| NMAP parameter (for ping)   | PE/PP/PM: ICMP echo, timestamp, and netmask request discovery probes<br>sP: Ping Scan - go no further than determining if host is online<br>PR: ARP Scan<br>sT: TCP Connect Scan |
<!-- cSpell:enable -->
## Unique checks (Used during import/export procedure only!)

| Option       | Value     |
| ------------ | --------- |
| Object title | Yes or No |
| Layer2 nets  | Yes or No |
| IP-addresses | Yes or No |
| Hostname     | Yes or No |

## Barcodes

| Option                     | Value             |
| -------------------------- | ----------------- |
| Display barcodes in i-doit | Yes or No         |
| Barcode form               | QR-Code<br>Code39 |

## Graphical interface

| Option                              | Value                    |
| ----------------------------------- | ------------------------ |
| Display empty values as             | String                   |
| String for separation of locations  | String                   |
| Location path orientation           | left (default)<br>right  |
| String for separation of connectors | String                   |
| Drag 'n' Drop of objects            | Yes or No                |
| Object type sorting                 | Alphabetically<br>Manual |

## Maximum lengths

| Option                        | Value |
| ----------------------------- | ----- |
| Dialog-Plus                   | Value |
| Object title in location path | Value |
| Full Length location path     | Value |

## Logbook

| Option                                                | Value     |
| ----------------------------------------------------- | --------- |
| Log detailed CMDB changes                             | Yes or No |
| Disable logbook commentary                            | Yes or No |
| Delete Logbook entries from purged objects completely | Yes or No |

## Templates

| Option                                   | Value              |
| ---------------------------------------- | ------------------ |
| Show template filter in object lists     | Yes or No          |
| Colorize template assignments/references | Yes or No          |
| With color                               | Colorpicker<br>Hex |

## Security

| Option                           | Value              |
| -------------------------------- | ------------------ |
| Permission system                | Inactive<br>Active |
| Minimum length of user passwords | Value              |
| Display passwords                | Yes or No          |
| Information about last login     | Inactive<br>Active |
| Sanitize input data              | Yes or No          |

## Logging

| Option           | Value     |
| ---------------- | --------- |
| Right-system Log | Yes or No |
| Exception Log    | Yes or No |
| CMDB Import      | Yes or No |

## Quickinfo (Link mouseover)

| Option            | Value                 |
| ----------------- | --------------------- |
| Cache expiration  | Minute<br>Hour<br>Day |
| Rows per category | Value                 |

## LDAP

| Option              | Value                                                                 |
| ------------------- | --------------------------------------------------------------------- |
| Standard LDAP group | Comma-separated list of group ids                                     |
| LDAP Config:        | JSON String                                                           |
| Salutation Mister   | Comma separated list with mapped values for LDAP salutation attribute |
| Salutation Misses   | Comma separated list with mapped values for LDAP salutation attribute |

## Report Manager

| Option         | Value                                                                                  |
| -------------- | -------------------------------------------------------------------------------------- |
| Default filter | ID<br>Title<br>Category<br>Generated by query editor<br>Variable Report<br>Description |

## Import

| Option                                                   | Value     |
| -------------------------------------------------------- | --------- |
| Cancel process on validation error?                      | Yes or No |
| Empty only the affected attributes on validation errors? | Yes or No |
| The CSV Import can overwrite the object type?            | Yes or No |
| Amount of rows to be imported in a batch                 | Value     |

## Search

| Option                                          | Value                                                      |
| ----------------------------------------------- | ---------------------------------------------------------- |
| Default search mode                             | Normal<br>Deep Search                                      |
| Activate fuzzy search                           | Yes or No                                                  |
| Automatic DeepSearch                            | Active<br>Active when no results are found.<br>Deactivated |
| Highlight the search string                     | Yes or No                                                  |
| Minimum search string length                    | Value                                                      |
| Show archived/deleted objects in search results | Yes or No                                                  |
| Show location paths in search results           | Yes or No                                                  |

## JDisc

| Option                  | Value                  |
| ----------------------- | ---------------------- |
| Threshold               | Quantity               |
| Threshold unit          | Days<br>Weeks<br>Month |
| Maximum import pause    | Time in Minutes        |
| Paused import behaviour | Cancel<br>Continue     |

## Language

| Option                         | Value             |
| ------------------------------ | ----------------- |
| Default language for new users | German<br>English |

## Notifications

| Option                | Value     |
| --------------------- | --------- |
| Skip expired licenses | Yes or No |

## Installed Add-on related settings

| Option                                                                                                                          | Value                                                                                                                           |
| ------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| [ISMS](../../../i-doit-add-ons/isms.md) Filter report views with location based rights                                          | Yes or No                                                                                                                       |
| [ISMS](../../../i-doit-add-ons/isms.md) Show risk flag                                                                          | Yes or No                                                                                                                       |
| [ISMS](../../../i-doit-add-ons/isms.md) Show risk title                                                                         | Yes or No                                                                                                                       |
| [Documents](../../../i-doit-add-ons/documents/index.md) Comment revisions                                                       | Yes or No                                                                                                                       |
| [Documents](../../../i-doit-add-ons/documents/index.md) Cache generated documents                                               | Yes or No                                                                                                                       |
| [Maintenance](../../../i-doit-add-ons/maintenance.md) Get email addresses from                                                  | Resolve contact groups and notify each person individually<br>Simply use the selected contacts without resolving contact groups |
| [Events](../../../i-doit-add-ons/events.md) Base64 Decode Event Parameters                                                      | Yes or No                                                                                                                       |
| [Check_MK](../../../i-doit-add-ons/checkmk.md) Tags may only consist of alphabetic characters, numbers, underscores and hyphens | Yes or No                                                                                                                       |
| [Workflows](../../../i-doit-add-ons/workflow.md) Hide checklists in my-doit area                                                | Yes or No                                                                                                                       |
| [IT-Grundschutz](../../../i-doit-add-ons/viva/index.md) URL-Prefix to IT-Grundschutz Compendium                                 | URL                                                                                                                             |
| [IT-Grundschutz](../../../i-doit-add-ons/viva/index.md) Upload folder for IT-Grundschutz Compendium                             | Directory path                                                                                                                  |
| [Relocate-CI](../../../i-doit-add-ons/relocate-ci.md) Remove the logical location after a object has been relocated physically. | Yes or No                                                                                                                       |
| [Relocate-CI](../../../i-doit-add-ons/relocate-ci.md) Update the physical location after a object has been relocated logically. | Yes or No                                                                                                                       |
| [Relocate-CI](../../../i-doit-add-ons/relocate-ci.md) Write logbook entries to all children of a relocated object.              | Yes or No                                                                                                                       |
| [Forms](../../../i-doit-add-ons/forms/index.md) Forms Server                                                                    | URL                                                                                                                             |
| [Forms](../../../i-doit-add-ons/forms/index.md) User name                                                                       | String                                                                                                                          |
| [Forms](../../../i-doit-add-ons/forms/index.md) API Key                                                                         | String                                                                                                                          |
