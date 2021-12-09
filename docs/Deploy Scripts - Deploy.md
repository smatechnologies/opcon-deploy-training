---
sidebar_label: 'Deploy Scripts - Deploy'
hide_title: 'false'
---

## Deploy - Scripts
    
### Script Deploy

<a href="imgdeploy/Deployimg019.png" target="_blank"><img src="imgdeploy/Deployimg019.png" width="500"></img></a>    

###### (Click Images to Enlarge)

* Scripts are Deployed into the OpCon Script Repository of the selected OpCon System using the **Script Deploy** Function

* During the Script Deploy Process a check is made for existing Script Information in the Repository:
  - Script Type
  - Script Runner
  - Version

* The Deploy Process will stop if there is a Script Type mismatch

* If the Script exists, the Latest Version of the Script in the OpCon Script Repository is retrieved

* If the Script Version already exists in the OpCon Script Repository, a **Script Match** is performed by comparing the stored ```MD5``` Hash Values
    - The Deploy function will stop if the Values do not match

* The Script Version is then insterted into the OpCon Script Repository along with any missing Versions
    - This ensures that the Version Number of the Script is consistent 
    - (If Current Version is 5 and Latest Version in OpCon Script Repository is 3, then Versions 4 and 5 will be inserted)

* When the Deploy Icon has been selected, the '**Select Scripts**' Dialog Screen appears 

<a href="imgdeploy/Deployimg020.png" target="_blank"><img src="imgdeploy/Deployimg020.png" width="500"></img></a>    

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

<a href="imgdeploy/Deployimg021.png" target="_blank"><img src="imgdeploy/Deployimg021.png" width="500"></img></a>    

* When a Server has been selected, the **Summary** Dialog Screen will appear

<a href="imgdeploy/Deployimg022.png" target="_blank"><img src="imgdeploy/Deployimg022.png" width="500"></img></a>    

* The User can enter a comment that will be saved with the Deployment Process

* The **Review result of deployment** Dialog Screen provides the results of the Process

<a href="imgdeploy/Deployimg023.png" target="_blank"><img src="imgdeploy/Deployimg023.png" width="500"></img></a>    

<a href="imgdeploy/Deployimg024.png" target="_blank"><img src="imgdeploy/Deployimg024.png" width="500"></img></a>    

### Browse 

* The **Browse** Function allows the OpCon Deploy User to view information about the Script Definition in the Repository

<a href="imgdeploy/Deployimg025.png" target="_blank"><img src="imgdeploy/Deployimg025.png" width="500"></img></a>    

* The information displayed is:
    * Script Name, Type, and _Each_ Version in the Repository
    * Description entered during Import Process
    * The OpCon System from which the Definition was imported
    * The Script creation Date and Last Update from the OpCon Repository
    * The Deploy User who performed the last action on the Record and Date

  <a href="imgdeploy/Deployimg026.png" target="_blank"><img src="imgdeploy/Deployimg026.png" width="500"></img></a>    

* The Definition can also be displayed by Right-Clicking **Version** and selecting **View Script Content** 
    * The Definition will appear in a pop-up window
    * Contents can be searched
    * Contents can be copied to the Clipboard by highlighting desired information and selecting **Copy to Clipboard**

<a href="imgdeploy/Deployimg027.png" target="_blank"><img src="imgdeploy/Deployimg027.png" width="500"></img></a>    

###### (Click Images to Enlarge)