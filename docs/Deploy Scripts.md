---
sidebar_label: 'Deploy Scripts'
hide_title: 'false'
---

## Deploy - Scripts

* Deploy Scripts are associated with Script Runners and Script Types

* A Script may have multiple Script **Runners**, but only a single Script **Type**

* Scripts are versioned in the OpCon Script Repository

* Each time a Script is updated in the OpCon Script Repository, a new Version is automatically created

* When Scripts are manually moved from one OpCon System to another, it is possible for Script Version numbers in the OpCon Script Repository of each OpCon System to become inconsistent

* When working with multiple OpCon Systems, Version numbers associated with a Script must be consistent across OpCon Deploy and all OpCon Script Repositories
    - OpCon Deploy provides a centralized Repository for all Scripts to ensure Versioning is consistent across the OpCon Deploy and OpCon Script Repositories


### Schedule Check-In Process for Script Information

* If the Script Information does not exist in the Repository it will be added with all Versions

* If the Script Information exists in the Repository
    - Script Type will be checked for a match and a matching Script Type will add all Versions
    - If the Type does not match, Import will be stopped

### Schedule/Package Deploy Process for Embedded Script Information

* If the Script does not exist in the OpCon Script Repository, it will be inserted with all Script Versions

* If the Script exists in the Repository
    - Script Type will be checked for a match and a matching Script Type will add all Versions
    - If the Type does not match, Deployment will be stopped


<a href="imgdeploy/Deployimg014.png" target="_blank"><img src="imgdeploy/Deployimg014.png" width="500"></img></a>    

###### (Click Image to Enlarge)