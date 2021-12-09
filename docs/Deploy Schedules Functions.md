---
sidebar_label: 'Deploy Schedules Functions'
hide_title: 'false'
---

## Deploy - Schedules Functions

### Schedules Import

* The Import process allows a User to select from which OpCon System the Definition should be Imported
  - The OpCon Deploy User Role determines from which Systems the User may Import
  - The OpCon User associated with the OpCon Deploy User determines which Schedule Definitions may be selected on the OpCon System
  - It is possible to select multiple Schedule Definitions to Import

* When the Import Icon is selected, the **Select a Server** Dialog Screen allows selection of an OpCon System from the drop-down list
  - The drop-down list will only present a list of OpCon Servers that are associated with the User's OpCon Deploy Role

<a href="imgdeploy/Deployimg029.png" target="_blank"><img src="imgdeploy/Deployimg029.png" width="500"></img></a>  

###### (Click Images to Enlarge)

* Once an OpCon System has been selected and its license is verified, the **Select a Schedule to Import** Dialog Screen will appear
  - A list of available Schedule Definitions will appear in the Left Dialog Box
  - Schedules can be selected for Import by highlighting them in the Left Dialog Box and using the ```>``` button to move selections to the Right Dialog Box

<a href="imgdeploy/Deployimg030.png" target="_blank"><img src="imgdeploy/Deployimg030.png" width="500"></img></a>  

:::note Note
_If the requested OpCon System has an ```Invalid``` License an error message will appear_
<a href="imgdeploy/Deployimg031.png" target="_blank"><img src="imgdeploy/Deployimg031.png" width="500"></img></a> 
:::

* Once selections are complete, all Definitions in the Right Dialog Box will be Imported into the Repository

<a href="imgdeploy/Deployimg032.png" target="_blank"><img src="imgdeploy/Deployimg032.png" width="500"></img></a>  

* Clicking the **Finish** button will begin the Import Process immediately

* Clicking the **Next** button advances to the Summary Dialog Screen
  - By default, the Import Process automatically selects Properties, Thresholds/Resources, and Calendar indicators fo the Schedule Definition
  - The User can enter a comment that will be added to the Schedule Record

<a href="imgdeploy/Deployimg033.png" target="_blank"><img src="imgdeploy/Deployimg033.png" width="500"></img></a>  

* If Selected Definitions contain OpCon **SAP R3** Definitions, selecting ```Refresh SAP Job Definitions``` will extract the SAP Job Definitions from the associated SAP Server

<a href="imgdeploy/Deployimg034.png" target="_blank"><img src="imgdeploy/Deployimg034.png" width="500"></img></a>  

* When the **Finish** button is selected, a **Progress Message** is displayed
  - When the Process is complete, a **Review result of check-in** Dialog Screen appears

<a href="imgdeploy/Deployimg035.png" target="_blank"><img src="imgdeploy/Deployimg035.png" width="500"></img></a>  

### Schedules Import - JSON

* It is possible to Import a correctly defined JSON Schedule Definition from a file in the Repository
  - When the Import File icon is selected, the **Import a schedule from a file** Dialog Screen appears
  - The file can be selected through browsing
  - If the Definition contains a Valid Header, the information will be displayed in the Description Section

<a href="imgdeploy/Deployimg036.png" target="_blank"><img src="imgdeploy/Deployimg036.png" width="500"></img></a>  

:::note Note
_If the file is not a Valid JSON Definition, an error message will appear_
<a href="imgdeploy/Deployimg037.png" target="_blank"><img src="imgdeploy/Deployimg037.png" width="500"></img></a>  
:::

### Schedules Import - Batch.SMAOpConDeployClient.exe

* Imports can be performed using the ```Batch.SMAOpConDeployClient.exe``` program
  - The program Imports a single Schedule by providing the Schedule Name
  - Multiple Schedules can be Imported using a File Name that contains a list of Schedule Names

```
C:\test\Batch.SMAOpConDeployClient.exe -s OPC170-PROD -w "SCHED001' -u admin -a IMPORT -p IBsC5ohnSf2P7/Ku81FiGw==
```

* An Initial Population of the Deploy Respository can be performed from a Production OpCon System using the ```Batch.SMAOpConDeployClient.exe``` program
  - The Process extracts the Schedules named in the Import File
  - The Schedule Record is created
  - The Deployment Record is created indicating that the Schedule Definition is Deployed to the Production System
  - The Definition is set as Current in Production

* The program is called from the Command line passing a set of Arguments

* ```Batch.SMAOpConDeployClient``` supports the following Import Arguments:
  - ```-a```  (required) action must be set to Import
  - ```-d```  (optional) description added to the Imported Record(s)
  - ```-fw``` (optional) defines the name of a file containing the names of Schedule Definitions to Import  (Either ```-fw``` or ```-w``` must be present)
  - ```-p```  the password of the Deploy User encrpypted using OpCon EM encryption
  - ```-s```  (required) the name of the OpCon System from which the Schedules must be Imported. The Server Name must be a defined Deploy Server
  - ```-u```  (required) the Deploy User performing the Import Operation
  - ```-w```  (optional) defines the name of a Workflow to Import (Either ```-w``` or ```-fw``` must be present)

### Schedules Import - Browse

* The Browse function allows the OpCon Deploy User to view information about the Schedule Definition in the Repository

<a href="imgdeploy/Deployimg039.png" target="_blank"><img src="imgdeploy/Deployimg039.png" width="500"></img></a>  

* The information displayed in the Browse function consists of:
  - Schedule Name and each Version in the Repository
  - Referenced SubSchedules in the Definition
  - Referenced External Dependencies in the Definition
  - Description entered during the Import Process
  - OpCon System from which the Definition was Imported

* The Definition can also be displayed by Right-Clicking on the Version and selecting **View Defintion** in the pop-up

<a href="imgdeploy/Deployimg040.png" target="_blank"><img src="imgdeploy/Deployimg040.png" width="500"></img></a>  

  - Definition will appear in a new pop-up window
  - Contents can be searched by entering a Value in the top search bar
  - Contents can be copied to the clipboard by highlighting what is required and selecting **Copy to Clipboard**

<a href="imgdeploy/Deployimg041.png" target="_blank"><img src="imgdeploy/Deployimg041.png" width="500"></img></a>  