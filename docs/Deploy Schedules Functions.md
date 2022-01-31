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

![Deployimg029](/imgdeploy/Deployimg029.png) 

* Once an OpCon System has been selected and its license is verified, the **Select a Schedule to Import** Dialog Screen will appear
  - A list of available Schedule Definitions will appear in the Left Dialog Box
  - Schedules can be selected for Import by highlighting them in the Left Dialog Box and using the ```>``` button to move selections to the Right Dialog Box

![Deployimg030](/imgdeploy/Deployimg030.png) 

:::note Note
_If the requested OpCon System has an ```Invalid``` License an error message will appear_
![Deployimg031](/imgdeploy/Deployimg031.png)
:::

* Once selections are complete, all Definitions in the Right Dialog Box will be Imported into the Repository

![Deployimg032](/imgdeploy/Deployimg032.png)

* Clicking the **Finish** button will begin the Import Process immediately

* Clicking the **Next** button advances to the Summary Dialog Screen
  - By default, the Import Process automatically selects Properties, Thresholds/Resources, and Calendar indicators fo the Schedule Definition
  - The User can enter a comment that will be added to the Schedule Record

![Deployimg033](/imgdeploy/Deployimg033.png)

* If Selected Definitions contain OpCon **SAP R3** Definitions, selecting ```Refresh SAP Job Definitions``` will extract the SAP Job Definitions from the associated SAP Server

![Deployimg034](/imgdeploy/Deployimg034.png) 

* When the **Finish** button is selected, a **Progress Message** is displayed
  - When the Process is complete, a **Review result of check-in** Dialog Screen appears

![Deployimg035](/imgdeploy/Deployimg035.png) 

### Schedules Import - JSON

* It is possible to Import a correctly defined JSON Schedule Definition from a file in the Repository
  - When the Import File icon is selected, the **Import a schedule from a file** Dialog Screen appears
  - The file can be selected through browsing
  - If the Definition contains a Valid Header, the information will be displayed in the Description Section

![Deployimg036](/imgdeploy/Deployimg036.png)

:::note Note
_If the file is not a Valid JSON Definition, an error message will appear_
![Deployimg037](/imgdeploy/Deployimg037.png)
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

![Deployimg039](/imgdeploy/Deployimg039.png)

* The information displayed in the Browse function consists of:
  - Schedule Name and each Version in the Repository
  - Referenced SubSchedules in the Definition
  - Referenced External Dependencies in the Definition
  - Description entered during the Import Process
  - OpCon System from which the Definition was Imported

* The Definition can also be displayed by Right-Clicking on the Version and selecting **View Defintion** in the pop-up

![Deployimg040](/imgdeploy/Deployimg040.png)

  - Definition will appear in a new pop-up window
  - Contents can be searched by entering a Value in the top search bar
  - Contents can be copied to the clipboard by highlighting what is required and selecting **Copy to Clipboard**

![Deployimg041](/imgdeploy/Deployimg041.png)