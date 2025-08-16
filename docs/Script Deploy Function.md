---
sidebar_label: 'Script Deploy Function'
---

## Overview

* Scripts are Deployed into the OpCon Script Repository of the selected OpCon System using the **Script Deploy** Function
    
## Script Deploy

* During the Script Deploy Process a check is made for existing Script Information in the Repository:
  * Script Type
  * Script Runner
  * Version

![Deployimg019](../static/imgdeploy/Deployimg019.png)

* The Deploy Process will stop if there is a Script Type mismatch
* If the Script exists, the Latest Version of the Script in the OpCon Script Repository is retrieved
* If the Script Version already exists in the OpCon Script Repository, a **Script Match** is performed by comparing the stored ```MD5``` Hash Values
  * The Deploy function will stop if the Values do not match
* The Script Version is then inserted into the OpCon Script Repository along with any missing Versions
  * This ensures that the Version Number of the Script is consistent 
  * (If Current Version is 5 and Latest Version in OpCon Script Repository is 3, then Versions 4 and 5 will be inserted)
* When the Deploy Icon has been selected, the '**Select Scripts**' Dialog Screen appears 

![Deployimg020](../static/imgdeploy/Deployimg020.png)  

*  The User can now select Scripts to Deploy
* It is possible to Deploy _multiple_ Scripts
* Script Versions are included by adding the Definition in the lower box of the Dialog Screen. 

The **Up** and **Down** Arrows between Dialog Boxes functions as specified below:
 
```Single Down``` **Adds** Individual Scripts to the Lower Dialog Box
 
```Single Up``` **Removes** Individual Scripts from the Lower Dialog Box
 
```Double Down``` **Adds** All Selections to the Lower Dialog Box
 
```Double Up``` **Removes** All Selections from the Lower Dialog Box


* Once Scripts have been selected, the **Next** Button will advance to the '**Select a Server**' Dialog Screen
    * The drop-down list will only present a list of OpCon Servers that are associated with the User's OpCon Deploy Role

![Deployimg021](../static/imgdeploy/Deployimg021.png)

* When a Server has been selected, the **Summary** Dialog Screen will appear

![Deployimg022](../static/imgdeploy/Deployimg022.png) 

* The User can enter a comment that will be saved with the Deployment Process

* The **Review result of deployment** Dialog Screen provides the results of the Process

![Deployimg023](../static/imgdeploy/Deployimg023.png)

![Deployimg024](../static/imgdeploy/Deployimg024.png)