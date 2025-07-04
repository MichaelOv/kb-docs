---
title: Example of CSV import - Licenses
description: Example of CSV import - Licenses
published: true
date: 2025-07-02T16:10:16.149Z
tags: 
editor: markdown
dateCreated: 2025-07-02T16:10:14.006Z
---

!!! warning "Please create a complete backup before making any changes to an interface/import. If the result is not satisfying, it can then be restored"

In this example we build on the [CSV import of applications](example-csv-import-applications.md) and want to import licenses.

!!! info "This article was last checked for i-doit version 34"

For the import we need the following information:

-   Object type → what type of object it should be.
-   Object title → the name of the client
-   License Assignment: License Key - License Type → Which license type will be imported, single or volume?
-   License Assignment: License Key - Number → What is the number of licenses?
-   License Assignment: License Key - Key → What is the license key?
-   License assignment: License key - Serial number → Which serial number should be assigned?
-   License assignment: License key - Start date → From when can the license be used?
-   License assignment: License key - Expiration date → When does the license expire?
-   License assignment: License key - Unit price → What does a license cost?

!!! info "With each import, the data format must also be taken into account."

For example:

[![example](../../assets/images/en/consolidate-data/csv-data-import/csv-import-licenses/1-csv-i-l.png)](../../assets/images/en/consolidate-data/csv-data-import/csv-import-licenses/1-csv-i-l.png)

Dialog titles in English are expected, for example: single-license.  
Here the date format YYYY-MM-DD (2021-11-26) is expected.  
And the numeric format: X,XXX,XX (1,111.11), because the comma is set by i-doit we only insert values like 12999.99.

Example CSV file for this import:

[Import-Licenses.csv :material-file-download:](../../assets/images/en/consolidate-data/csv-data-import/csv-import-licenses/Import-Licenses.csv){ .md-button .md-button--primary }

??? example "Import Licenses.csv"
    ```text
    Object type;Object title;Licenses: License keys > License Type (Dialog);Licenses: License keys > Amount;Licenses: License keys > Key;Licenses: License keys > Serial;Licenses: License keys > Start Date (Date);Licenses: License keys > Expiration Date (Date);Licenses: License keys > Price Per Unit (Money)
    C__OBJTYPE__LICENCE;License-X;Volume license;1000;License-X-111-LASKDZHW;123456789;2021-01-01;2021-12-31;999.9
    C__OBJTYPE__LICENCE;License-Y;Single license;1;License-Y-211-OIHUASFD;1123456789;2021-06-01;2021-12-31;1399.9
    C__OBJTYPE__LICENCE;License-Z;Volume license,Volume license;100,50;License-Z-311-IGUHOPSD,License-Z-322-IUHGASD;11123456789,11223456789;2021-01-01,2021-05-01;2021-12-31,2021-04-30;10200.9,500.9
    ```

No dependencies are assumed for this import.

For the import we go back to the CSV import area. We set "Multi-valued categories" to "Comma-separated".

[![import](../../assets/images/en/consolidate-data/csv-data-import/csv-import-licenses/2-csv-i-l.png)](../../assets/images/en/consolidate-data/csv-data-import/csv-import-licenses/2-csv-i-l.png)

Now we can make the import configuration in the lower area as follows and then start the import process::

[![import-start](../../assets/images/en/consolidate-data/csv-data-import/csv-import-licenses/3-csv-i-l.png)](../../assets/images/en/consolidate-data/csv-data-import/csv-import-licenses/3-csv-i-l.png)

If you have done everything correctly, the licenses will now appear in the list view.

[![licenses](../../assets/images/en/consolidate-data/csv-data-import/csv-import-licenses/4-csv-i-l.png)](../../assets/images/en/consolidate-data/csv-data-import/csv-import-licenses/4-csv-i-l.png)

Also, the License Assignment and License Assignment: License Key categories are filled.

[![license-key](../../assets/images/en/consolidate-data/csv-data-import/csv-import-licenses/5-csv-i-l.png)](../../assets/images/en/consolidate-data/csv-data-import/csv-import-licenses/5-csv-i-l.png)

[![license-key](../../assets/images/en/consolidate-data/csv-data-import/csv-import-licenses/6-csv-i-l.png)](../../assets/images/en/consolidate-data/csv-data-import/csv-import-licenses/6-csv-i-l.png)

## Importing objects with volume licenses

If you want to import an object that is supposed to have a volume license and license key assigned, you can achieve this by using the software assignment category and changing the csv syntax as follows:

[Volume-Licenses.csv :material-file-download:](../../assets/images/en/consolidate-data/csv-data-import/csv-import-licenses/Volume-Licenses.csv){ .md-button .md-button--primary }

??? example "Volume-License.csv"
    ```text
    Title; "Application";License key
    DESKTOP-XMS3R8;"Windows 8 Development Essentials";"Development;MDW-4253-1257"
    DESKTOP-DK2MD9L;"Windows 10 Pro";"Professional;EVT-2024-9931"
    ```

The mapping for the csv-file should be set as follows:

[![license-key](../../assets/images/en/consolidate-data/csv-data-import/csv-import-licenses/7-csv-i-l.png)](../../assets/images/en/consolidate-data/csv-data-import/csv-import-licenses/7-csv-i-l.png)

[![license-key](../../assets/images/en/consolidate-data/csv-data-import/csv-import-licenses/8-csv-i-l.png)](../../assets/images/en/consolidate-data/csv-data-import/csv-import-licenses/8-csv-i-l.png)

Once the import has been successfully completed, a new entry can be found in the Software assignment category of the imported object, in which both the license and the key are specified.

[![license-key](../../assets/images/en/consolidate-data/csv-data-import/csv-import-licenses/9-csv-i-l.png)](../../assets/images/en/consolidate-data/csv-data-import/csv-import-licenses/9-csv-i-l.png)
