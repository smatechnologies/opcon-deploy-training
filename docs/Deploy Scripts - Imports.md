---
sidebar_label: 'Deploy Scripts - Imports'
hide_title: 'false'
---

## Deploy - Scripts
    
### Script Import


* Scripts are imported into the Repository with the **Script Import** Capability

![Deployimg015](/imgdeploy/Deployimg015.png)

* During the Script Import Process a check is made for existing Script Information in the Repository:
  - Script Type
  - Script Runner
  - Version

* If the Script exists, a check is made to ensure the Script Type Values in the Repository match the Definition Values
  - The Import Process will stop if there is a mismatch

* If the Script Type matches, a check is made to see if the Version already exists in the Repository

* If the Version does not exist, a check is made to see if there are any missing versions between the latest Value in the Repository and the New Version
  - If there are missing versions, those versions will be extracted from the same OpCon System from which the New Version is being imported, ensuring that Version numbers in the Repository are consistent

* When the Import icon has been selected, the '**Select a Server**' dialog appears allowing the User to select an OpCon System from the dropdown list
  - The dropdown list will only present a list of OpCon Servers that are associated with the User's OpCon Deploy Role

* When the ```Next``` button has been selected in the dialog box, the '**Select one or more Scripts to import**' dialog appears

![Deployimg016](/imgdeploy/Deployimg016.png) 

  - A list of available Script Definitions appears in the Left-Hand box
  - The column '**Nb Versions**' indicates how many Versions of the Script are present in the OpCon Script Repository
  - Scripts can be selected for Import by marking them in the Left-Hand box and pressing the '**>**' button to add the selections to the Right-Hand box

* Once the selections are complete, all Definitions in the Right-Hand box will be Imported into the Repository

* When the ```Next``` button has been selected in the dialog box, the '**Summary**' dialog appears with User selections

![Deployimg017](/imgdeploy/Deployimg017.png)

  - Comments can be added to the Schedule Record in the '**Summary**' dialog

* When the ```Finish``` button has been selected a **Progress Message** is displayed and when the process completes, the '**Review result of check-in**' dialog will appear

![Deployimg018](/imgdeploy/Deployimg018.png)   