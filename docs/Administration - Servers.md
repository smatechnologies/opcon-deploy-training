---
sidebar_label: 'Administration - Servers'
hide_title: 'false'
---

## Deploy Administration - Servers

* Servers are used to define OpCon systems that will participate in OpCon Deploy Operations

* Servers are allocated a **Type** which determines its function in the Deploy environmnet
    - Connections to OpCon Systems should support TLS connections using Self-Signed Certificates
    - Each Server requires a Deploy License which is checked before executing any requests on a System

### Server Definition Requirements

![Deployimg006](/imgdeploy/Deployimg006.png)

* Server Definition Requirements
    - Defined Port Number for the Deploy Server 
    - Defined Port Number for the OpCon-API server associated with the OpCon System
    - Server Name must be unique within the Deploy Environment
    - Each server must be assigned a Server Type
    - **Allows Transformation Rules** can be toggled on or off

### Server Types

* Server Types are associated with User Roles and determine allowed User Actions on the OpCon System
    - Development
    - Integration
    - Pre-Production
    - Production
    - Quality Assurance
    - System Test
    - Training
    - Test

### Server Transformation Rules

* Default Transformation Rules can be associated with the OpCon System
    - When a deployment takes place, these Transformation Rules will automatically be applied to the specified Package/Schedule Definitions
    - This allows options such as Machine Names, Machine Group Names, Batch Users, etc. to be transformed automatically for each OpCon System

* Multiple Definitions can be assigned by Double-Clicking each desired item

![Deployimg007](/imgdeploy/Deployimg007.png)

* Contents of the Definition can be viewed using Right-Click

![Deployimg008](/imgdeploy/Deployimg008.png)

### SAP Server Support

* If the environment contains SAP R3 Systems and automated linking of OpCon SAP Job Definitions to SAP Jobs in required, SAP Systems must be defined
    - It is also possible to extract SAP Job Definitions from an SAP System and create the Jobs in a target SAP System

* SAP Server Support Options/Requirements:
    - **SAP Server Name** (The Name of the SAP Agent)
    - **Language** (The Language Code; eg **EN**, **F**)
    - **SAP User** (The User Code required by the SAP Agent to communicate with the SAP Server)
    - **SAP External User** (Same as SAP User)
    - **Password** (SAP User Password in plain text which will be encrypted by the software)

![Deployimg009](/imgdeploy/Deployimg009.png)

![Deployimg010](/imgdeploy/Deployimg010.png)

### Batch Schedule Server

![Deployimg011](/imgdeploy/Deployimg011.png)

* The BatchScheduleServer is a special server Definition used to drive Batch Deployment
* Deploy uses the OpCon-API to add a Job to the BATCH-DEPLOY Schedule to perform future deployment
* Deploy will also ensure that a BATCH-DEPLOY Schedule is available for the required day
    - If a Schedule is not available for the required day, a Schedule Build will be submitted