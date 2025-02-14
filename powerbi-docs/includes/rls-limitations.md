---
author: mgblythe
ms.service: powerbi
ms.topic: include
ms.date: 09/13/2019
ms.author: mblythe
---

## Limitations

Following is a list of the current limitations for row-level security on cloud models.

* If you previously defined roles and rules in the Power BI service, you must re-create them in Power BI Desktop.

* You can define RLS only on the datasets created with Power BI Desktop. If you want to enable RLS for datasets created with Excel, you must convert your files into Power BI Desktop (PBIX) files first. [Learn more](../desktop-import-excel-workbooks.md)

* Only Import and DirectQuery connections are supported. Live connections to Analysis Services are handled in the on-premises model.

## Known issues

There is a known issue where you'll get an error message if you try to publish a previously published report from Power BI Desktop. The scenario is as follows.

1. Anna has a dataset that is published to the Power BI service and has configured RLS.

1. Anna updates the report in Power BI Desktop and republishes.

1. Anna receives an error.

**Workaround:** Republish the Power BI Desktop file from the Power BI service until this issue is resolved. You can do that by selecting **Get Data** > **Files**.
