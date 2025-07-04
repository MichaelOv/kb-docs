---
title: release-notes-119
description: 
published: true
date: 2025-07-02T16:18:46.188Z
tags: 
editor: markdown
dateCreated: 2025-07-02T16:18:43.905Z
---

We're happy to announce our latest major version 1.19 of i-doit. This release is a very important step in the development of i-doit. See the changelog for a complete list of changes. We encourage you to [update](../../maintenance-and-operation/update.md) to this release as soon as possible.

Highlights in this release
--------------------------

-   A complete **redesign** of the i-doit frontend to **improve the user experience**.
-   Added **compatibility** for **PHP 8.0**.
-   **New configuration** to **create custom translations** and **custom languages**.
-   **Setting** to define a [**default language**](../../system-administration/administration/tenant-management/settings-for-tenant.md#language) for newly created users.
-   **New configuration** to **[attribute settings](../../system-administration/administration/data-view/attribute-settings.md)** from categories and/or overview pages.
-   **Option** to **log** the **[last login](../../system-administration/administration/tenant-management/settings-for-tenant.md#security)** of a user.
-   [**Export** for **reports**](../../evaluation/report-manager.md#exportimport-reports) which have been created via **query builder**.

Add-ons
-------

!!! warning
    The New Add-on Versions require i-doit >= 1.19

Alongside i-doit 1.19, we will also release new versions of the following **add-ons**, which **need to be updated** afterwards to be compatible with **PHP 8.0** and the **new design**:

-   [API](../../i-doit-add-ons/api/index.md) **1.13**
-   [Documents](../../i-doit-add-ons/documents/index.md) **1.5**
-   [Analysis](../../i-doit-add-ons/analysis.md) **1.3**
-   [Floorplan](../../i-doit-add-ons/floorplan.md) **1.6**
-   [Cabling](../../i-doit-add-ons/cabling.md) **1.2**
-   [Relocate CI](../../i-doit-add-ons/relocate-ci.md) **1.2**
-   [Replacement](../../i-doit-add-ons/replacement.md) **1.4**
-   [Maintenance](../../i-doit-add-ons/maintenance.md) **1.2**
-   [Events](../../i-doit-add-ons/events.md) **1.3**
-   [Workflow](../../i-doit-add-ons/workflow.md) **1.1**
-   [Checkmk](../../i-doit-add-ons/checkmk.md) **1.1**
-   [Check\_MK 2](../../i-doit-add-ons/checkmk2/index.md) **1.8**
-   [Nagios](../../i-doit-add-ons/nagios.md) **1.1**
-   [Packager](../../i-doit-add-ons/add-on-packager.md) **1.2**

Important update notes
----------------------

-   With i-doit 1.19, **PHP 7.3** is **no longer supported**. Please ensure to upgrade to **PHP 7.4** first before updating to i-doit 1.19. Do **not** upgrade to **PHP 8.0** as long as you are using **i-doit < 1.19**.<br>
-   **After** the update of i-doit 1.19, you are free to upgrade PHP to 8.0 which is also **highly recommended**.<br>
-   **Before activating** the feature to log the **last login of a user**, please check whether this is compatible with the **data protection agreements** of your company and country. Contact your data privacy expert first if you are not sure about this.<br>
-   If you want to use the **new icons** for object types after updating to i-doit 1.19, you can activate them manually in your i-doit **administration** under System tools > Cache / Database.<br>
-   The following **Partner Add-ons** need to be updated **before** the i-doit 1.19 update (If these version requirements are not matched, the i-doit update cannot be performed):<br>
    -   **[ISMS](../../i-doit-add-ons/isms.md)** needs to be updated to version **1.5.2 or higher**
    -   **[VIVA 2](../../i-doit-add-ons/viva2.md)** needs to be updated to version **3.2.1 or higher**
    -   **Privacy** needs to be updated to version **1.1 or higher**
    -   **Label** needs to be updated to version **0**.5**or higher**
    -   **Disposal** needs to be updated to version **1.1.2** **or higher**
    -   **Inheritance** needs to be updated to version **1.3.7** **or higher**

System requirements
-------------------

Please check that your system matches the [system requirements](../../installation/system-requirements.md) before updating your instance to i-doit 1.19. Please also check that you have created a [backup of all your data](../../maintenance-and-operation/backup-and-recovery/index.md) and all add-ons are [up-to-date](../../i-doit-add-ons/index.md).
