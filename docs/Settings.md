---
sidebar_label: 'Settings'
hide_title: 'false'
---

## Administration - Settings

* Deploy Settings are used to define Global Settings and Global Rules in the OpCon Deploy Environment
  * These settings override options selected by Users during Operations

### Global Settings

* **Number of Versions to Retain**
  * Defines the number of Versions to keep in the Main Tables during the Archiving process

### Global Rules

![Deployimg012](../static/imgdeploy/Deployimg012.png)

* **Update Properties Allowed**
  * Defines whether or not Global Property values can be updated during the deployment process
* **Update Variables Allowed**
  * Defines whether or not Resource and Threshold values can be updated during the deployment process
* **Update Schedule Instance Properties**
  * Defines whether or not Schedule Instance Property values can be updated during the deployment process
* **Fail If A Dependency Is Not Present**
  * Defines whether or not the deployment process should **Fail** if an External Dependency (Cross Schedule Dependency)  is missing
* **Fail If Transformation Rules Are Present and Transformation Disabled**
  * Defines whether or not the deployment process should **Fail** if a user selects Transformation Rules and the target system does not support Transformation Rules
* **Add Package Name as Job Tag**
  * Defines whether or not the Package Name should be added to all jobs associated with the Package during deployment process
* **Delete Schedule From Development System After Import**
  * If Enabled, the definition will be deleted when a schedule from an OpCon system that has been designated as a Development system is imported into the Repository
