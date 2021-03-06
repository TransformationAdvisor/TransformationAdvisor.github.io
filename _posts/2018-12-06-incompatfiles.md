---
layout: post
title: Error during upload - INCOMPATIBLE FILES DETECTED
categories: Upload
author: Niall Horgan
---

The data collector produces reports that are linked to each application
In this case the process to link the report to an application has failed
This means one or more applications were not processed correctly

You can resolve this issue as follows:
```
1. Explode the profile.zip file
2. Delete files with the following names: 
     InventoryReport.json, InventoryReport.html, AnalysisReport.json, 
     AnalysisReport.html, TechnologyReport.json, TechnologyReport.html
3. Manually upload the zip file to Transformation Advisor through the UI
```
You may be missing some applications. To determine missing applications :
```
1. Get the list of applications in Transformation Advisor
2. Look at the profiles directory in <WAS_HOME> to see the full list of applications 
   installed in that profile
3. Identify applications in the profile that are missing from Transformation Advisor
```
