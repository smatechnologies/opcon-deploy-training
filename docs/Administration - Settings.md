---
sidebar_label: 'Administration - Settings'
hide_title: 'false'
---

## Deploy Administration - Settings

* Deploy Settings are used to define Global Settings and Global Rules in the OpCon Deploy Environment
    - These settings override options selected by Users during Operations

### Global Settings

* Number of Versions to retain
    - Defines the number of Versions to keep in the Main Tables during the Archiving process

### Global Rules

![Deployimg012](../static/imgdeploy/Deployimg012.png)

* **Update Properties Allowed**
    - Defines whether or not Global Property Values can be updated during the Deploy process

* **Update Variables Allowed**
    - Defines whether or not Resource and Threshold Values can be updated during the Deploy process

* **Update Schedule Instance Properties**
    - Defines whether or not Schedule Instance Property Values can be updated during the Deploy process

* **Fail If A Dependency Is Not Present**
    - Defines whether or not the Deploy process should **Fail** if an External Dependency is missing

* **Fail If Transformation Rules Are Present and Transformation Disabled**
    - Defines whether or not the Deploy process should **Fail** if a User selects Transformation and the Target OpCon System does not support Transformation

* **Add Package Name as Job Tag**
    - Defines whether or not the Package Name should be added to all tasks associated with the Package during deployment

* **Delete Schedule From Development System After Import**
    - If Enabled, the Definition will be deleted when a Schedule from an OpCon system that has been designated as a Development system is imported into the Repository
