---
title: changelog-117
description: 
published: true
date: 2025-07-02T16:36:06.297Z
tags: 
editor: markdown
dateCreated: 2025-07-02T16:36:04.042Z
---

# Changelog 1.17
<!-- cSpell:disable -->
<!-- markdownlint-disable MD052 -->
[Improvement][Categories] New license type "CPU core-based"<br>
[Improvement][Categories] Calculation for licenses of type "CPU core based"<br>
[Improvement][Custom categories] Configuration to manually design the structure of labels and fiels of custom categories<br>
[Improvement][Lists] Filtering for empty field in object lists<br>
[Improvement][Lists] Filter for empty values in object lists<br>
[Improvement][Lists] Filter for empty values in object lists<br>
[Improvement][Logbook] Full information for changes in backwards categories<br>
[Bug][Categories] Changes on the overview page create an empty entry in the category "software assignment" if this catgory is used on the overview page and the object has an assigned operating system<br>
[Bug][Categories] Apache2 is completely used up if a free IP address is searched for but there is no free IP address in the selected address allocation.<br>
[Bug][Categories] The search domain is not added when the network is changed<br>
[Bug][Categories] ##COUNT## Placeholder is not evaluated for outputs (connection)<br>
[Bug][Categories] Description of category "Emergency Plan" (Folder) is not forwarded to category "Emergency plan properties"<br>
[Bug][Categories] "Export as CSV" button is missing in category Applications > Installation<br>
[Bug][Categories] Assignment of persons to person groups is not shown properly<br>
[Bug][Categories] CSV import: Application category is not displayed for the Application object type<br>
[Bug][Custom categories] For the "Date and time" field type, the time is not displayed in the object list<br>
[Bug][Custom categories] Custom category not usable if attributes have backslashes in title<br>
[Bug][Update] Backup config files accessable<br>
[Bug][CSV Import] Values in user-defined categories are not overwritten by the CSV import option "Overwrite empty values<br>
[Bug][CSV Import] CSV Import: When a profile is saved, the last profile in the list is always selected.<br>
[Bug][CSV Import] CSV import escaped no "special characters<br>
[Bug][CSV Import] Missing configuration of the "Number of lines per import batch" count<br>
[Bug][JDisc] JDisc: "old" logic for databases is not imported correctly<br>
[Bug][JDisc] Clusters imported via JDisc are machted only by their name<br>
[Bug][Code (internal)] Cable connections are not displayed when inputs and outputs are connected<br>
[Bug][Code (internal)] Calling a license key entry with less than (<) characters blocks the use of the Licenses > License Assignment >> License Keys category<br>
[Bug][Code (internal)] Uploaded files with an umlaut as initial letter cannot be downloaded<br>
[Bug][Code (internal)] When deleting object images the folders should also be deleted if they are empty.<br>
[Bug][Lists] Using a default sorting for object lists causes an error<br>
[Bug][Lists] Attribute selection for category list of category "software assignment" incomplete<br>
[Bug][Lists] Sorting the attribute "Salutation" in object list causes an error<br>
[Bug][Logbook] Instead of the object name the logbook contains only the ID<br>
[Bug][Report-Manager] Using attribute "Net" from category "Hostaddress" in report manager causes an error<br>
[Bug][Report-Manager] Report Manager: When using the category Service Assignment > Attribute Service there is an SQL error message<br>
[Bug][Report-Manager] When sorting by object type (General) in the report, a 500 error is displayed<br>
[Bug][Report-Manager] Sub category "persons" of category "organization" can not supply linked attributes<br>
[Bug][Report-Manager] Report Manager: using people group membership as a condition generates SQL error message<br>
[Bug][Report-Manager] Managed devices of a remote management conroller cannot be selected in the report<br>
[Bug][Report-Manager] The attribute Assigned Layer-3-net of the category Layer-2-Net ist not selectable in reports<br>
[Bug][Authorization system] Permissions of person groups are still active, even if the person group is archived or deleted<br>
[Bug][Authorization system] The permission to create objects is not inherited for person group editor<br>
[Bug][Authorization system] Display error for the permissions "archive" and "delete" for "reports in category<br>
[Bug][Authorization system] Removing LDAP right removes access to user-defined categories<br>
[Bug][Notifications] Notifications can be created without the create permission<br>
[Bug][Validation] The category Contract cannot be edited via list editing if validation is activated for the attribute "Runtime unit".<br>
[Bug][Validation] Validation for category host address automatically assigns a new IP address although it should be blocked<br>
[Bug][CMDB] Sort by object count in object list configuration does not sort correctly<br>
[Bug][CMDB] Display error after aborting editing of the "General" category<br>
[Bug][List editing] Right "categories in object type" does not enable to modify content in list edit<br>
[Bug][LDAP] Login with an LDAP user generates error messages in the exceptions.log file<br>
[Bug][Import] Target schema (category: software assignment) cannot be filled via CSV import<br>
[Bug][Import] Active Directory computer import does not offer a choice of which object type to import as<br>
