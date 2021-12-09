---
sidebar_label: 'Deploy Deployment Schedules'
hide_title: 'false'
---

## Deployment - Schedule

<a href="imgdeploy/Deployimg056.png" target="_blank"><img src="imgdeploy/Deployimg056.png" width="600"></img></a> 

###### (Click Images to Enlarge)

### Deploying a Schedule

* The Deploy Process allows a User to:
  * Select a Schedule or Package to Deploy
  * Deploy the selection to available OpCon Systems
  * Add Transformation Rules
  * Determine if a Deployment, Simulation, or Batch Deployment must be performed

* Once the Deploy Icon has been selected on the Main Menu Screen, the **Select a Deployment Type** Dialog Screen appears

<a href="imgdeploy/Deployimg057.png" target="_blank"><img src="imgdeploy/Deployimg057.png" width="500"></img></a> 

* When **Schedule** is selected, the **Select a Schedule to Deploy** Dialog Screen appears

<a href="imgdeploy/Deployimg058.png" target="_blank"><img src="imgdeploy/Deployimg058.png" width="500"></img></a> 

  * When a Schedule is selected in the Upper Dialog Box, available Versions will be displayed in the Lower Dialog Box
  * The Definition can be displayed by Right*Clicking the Version and selecting **View Definition**

<a href="imgdeploy/Deployimg059.png" target="_blank"><img src="imgdeploy/Deployimg059.png" width="500"></img></a> 

* When the Version is selected and the screen is advanced, the **Select a Server** Dialog Screen appears

<a href="imgdeploy/Deployimg060.png" target="_blank"><img src="imgdeploy/Deployimg060.png" width="500"></img></a> 

  * A Server must be selected from the drop*down list

* Advancing the screen allows selection of Transformation Rules

<a href="imgdeploy/Deployimg061.png" target="_blank"><img src="imgdeploy/Deployimg061.png" width="500"></img></a> 

  * A Transformation Rule can be **Applied** by Double*Clicking the Version in the Upper Dialog Box
  * A Transformation Rule can be **Removed** by Double*Clicking the Verion in the Lower Dialog Box
  * The contents of the Rule can be seen by highlighting the Rule, Right*Clicking, and selecting **View Definition**

<a href="imgdeploy/Deployimg062.png" target="_blank"><img src="imgdeploy/Deployimg062.png" width="500"></img></a> 

* Advancing the screen allows selections within the **Build Options and Summary** Dialog Screen
  * **Auto Build** and **Auto Delete** settings can be selected

<a href="imgdeploy/Deployimg063.png" target="_blank"><img src="imgdeploy/Deployimg063.png" width="500"></img></a> 

  * Users can add comments for Deployment
  * Rebuild Schedules in the Daily can be selected
    * If the Schedule is already built in the Daily it will be rebuilt from the Current Date Forward (If the schedule is Active it cannot be rebuilt on Deployment)
  * SAP Job Definitions can be inserted from this screen as well
    * If SAP R3 Job Definitions are encountered in the System, they will be created in the SAP System and the OpCon SAP Job and SAP Job will be linked
    * If the option is not selected but SAP R3 Job Definitions are encountered, the System will link the OpCon SAP Job and the SAP Job

### Deploying a Package

<a href="imgdeploy/Deployimg057.png" target="_blank"><img src="imgdeploy/Deployimg057.png" width="500"></img></a> 

* When **Package** is selected from the **Select a Deployment Type** Dialog Screen, the **Select a Package to Deploy** Dialog Screen appears

<a href="imgdeploy/Deployimg064.png" target="_blank"><img src="imgdeploy/Deployimg064.png" width="500"></img></a> 

  * Available Versions are displayed in the Lower Dialog Box 
  * The number of Schedules in the Package are indicated

* Once the User selects a Package Version, the **Select a Server** Dialog Screen appears

<a href="imgdeploy/Deployimg060.png" target="_blank"><img src="imgdeploy/Deployimg060.png" width="500"></img></a> 

  * When a Server is chosen, the **Next** button advances to the **Select Transformation Rules** Dialog Screen

<a href="imgdeploy/Deployimg079.png" target="_blank"><img src="imgdeploy/Deployimg079.png" width="500"></img></a>   

* A Transformation Rule can be applied by Double*Clicking the desired Version in the Upper Dialog Box
  * The contents of the Transformation Rule can be seen by Right*Clicking the Rule and selecting **View Definition**

<a href="imgdeploy/Deployimg065.png" target="_blank"><img src="imgdeploy/Deployimg065.png" width="500"></img></a>   

* Advancing the screen allows the selections within the **Build Options and Summary** Dialog Screen

<a href="imgdeploy/Deployimg063.png" target="_blank"><img src="imgdeploy/Deployimg063.png" width="500"></img></a> 

  * **Auto Build** and **Auto Delete** settings can be selected
  * Users can add comments for Deployment
  * Rebuild Schedules in the Daily can be selected
    * If the Schedule is already built in the Daily it will be rebuilt from the Current Date Forward (If the schedule is Active it cannot be rebuilt on Deployment)
  * SAP Job Definitions can be inserted from this screen as well
    * If SAP R3 Job Definitions are encountered in the System, they will be created in the SAP System and the OpCon SAP Job and SAP Job will be linked
    * If the option is not selected but SAP R3 Job Definitions are encountered, the System will link the OpCon SAP Job and the SAP Job
