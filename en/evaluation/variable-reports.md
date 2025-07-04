---
title: Variable report
description: Variable report
published: true
date: 2025-07-02T15:54:57.938Z
tags: 
editor: markdown
dateCreated: 2025-07-02T15:54:55.749Z
---

Variable reports are very useful to customize your own i-doit installation for your individual needs.

## Example department printer

A lot of users already use the [custom categories](../basics/custom-categories.md). One thing which characterizes the custom categories is the possibility to link [objects](../basics/structure-of-the-it-documentation.md).

To give an example: Say that your company uses printers which are assigned to certain offices. The rooms **1.01** to **1.07** use **HQ Staff Printer 01**, rooms **1.0****8** to **1.11** use **HQ Staff Printer 02**.

This can be documented with the custom category **Department printer**. This category is assigned to the [object type](../basics/structure-of-the-it-documentation.md) **Printer** and defined as [single-value category](../basics/structure-of-the-it-documentation.md). The **Department printer for** [attribute](../basics/structure-of-the-it-documentation.md)  is added as **Object-Relation (Several objects)** with the addition **Share Access**.

[![Object-Relation](../assets/images/en/evaluation/variable-reports/1-vr.png)](../assets/images/en/evaluation/variable-reports/1-vr.png)

Then open the object **HQ Staff Printer 01**. Now you can select the assigned rooms in the **Department printer** category.

[![Printer](../assets/images/en/evaluation/variable-reports/2-vr.png)](../assets/images/en/evaluation/variable-reports/2-vr.png)

The result in the category is shown in the following picture.

[![category](../assets/images/en/evaluation/variable-reports/3-vr.png)](../assets/images/en/evaluation/variable-reports/3-vr.png)

You can also visualize the result with the [CMDB explorer](./cmdb-explorer/index.md).

[![CMDB explorer](../assets/images/en/evaluation/variable-reports/4-vr.png)](../assets/images/en/evaluation/variable-reports/4-vr.png)

But when you have a look at room **1.05** now, how can you find out which printer is assigned to this room? For this purpose, you need a "mirrored view" with which you can see which printer is related to this room. The variable report provide a good solution for such context-related queries.

To this end, you set up a [report](./report-manager.md) and another custom category. First, you create the report **Assigned department printer**. Select some significant **attributes** regarding the printers for the **Output**. The query builder provides the possibility to set a **Placeholder** for all links which generate relations under **Conditions**.

In our case this means: The report "searches" for those objects in which the [object ID](../basics/unique-references.md) of the currently selected object is listed in the custom category **Department printer** in the attribute **Department printer for**. But what is the selected object? There is no selected object in the context of the report manager.  This turns the report into a variable report.

[![Report](../assets/images/en/evaluation/variable-reports/5-vr.png)](../assets/images/en/evaluation/variable-reports/5-vr.png)

Therefore, an object must always be selected in order to populate the report. In this case you can achieve this by creating a category for the report which executes the report within an object. This is called **Department**, assigned to the object **Room** and defined as single-value category. There also is an unnamed attribute with the **Field type Report**. The ID of the above mentioned report is specified under **Addition**.

[![Field type Report](../assets/images/en/evaluation/variable-reports/6-vr.png)](../assets/images/en/evaluation/variable-reports/6-vr.png)

The report ID is contained in the overview of the already defined reports.

[![Field type Report](../assets/images/en/evaluation/variable-reports/7-vr.png)](../assets/images/en/evaluation/variable-reports/7-vr.png)

Now the new category is available in room objects. It always generates the report for the object in which the user currently is. By this means, you get a mirrored view of the relation to the department.

[![Field type Report](../assets/images/en/evaluation/variable-reports/8-vr.png)](../assets/images/en/evaluation/variable-reports/8-vr.png)
