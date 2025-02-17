---
content-type: faq
product-area: reporting
navigation-topic: tips-tricks-and-troubleshooting-reports
title: Data from shared columns not displayed in dashboard reports
description: Data from shared columns does not display when the report is placed in a multiple column dashboard layout, but it does display on a single column layout. Line breaks are also overridden.
author: Nolan
feature: Reports and Dashboards
---

# Data from shared columns not displayed in dashboard reports

## Problem

Data from shared columns does not display when the report is placed in a multiple column dashboard layout, but it does display on a single column layout. Line breaks are also overridden.

## Cause

Only columns marked as 

```
shortview=true
```

are included in the dashboard view of the report when the dashboard layout has the left/right split or the left/middle/right split set up.

## Solution

Access the view used in the report and open text mode. (For more information, see [Edit a view using text mode](../../../reports-and-dashboards/reports/text-mode/edit-text-mode-in-view.md).) Label all columns in the report, including the columns used in a shared/merged column, with 

```
shortview=true
```

. The report columns will then display properly in the dashboard.
