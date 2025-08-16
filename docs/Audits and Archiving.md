---
sidebar_label: 'Audits And Archiving'
---

## Overview

* Deploy includes an Audit Capability that captures messages when operations are performed
* These messages include:
  * User
  * Description of Message Capture
  * Time Stamp
* The messages are written into the Audit Table and can be viewed by any Administration Role

![Deployimg013](../static/imgdeploy/Deployimg013.png)

## Auditing

* **Audit Categories**
  * Deployment
  * Package
  * Schedule
  * Server
  * User
  * Global Rule
  * Script
  * Transformation Rule
* **Messages can be filtered by**
  * Category
  * User
  * Message Content
  * Date Range

## Archiving

* To maintain performance, it is necessary to perform archiving of unused Schedule, Package, and Transformation Rule Versions
  * The **Number of Versions to keep** setting defines how many version to keep
* If a Definition is still marked as **Active**, it **cannot** be Archived
* The **Archive process** moves Definitions from the **Main Tables** to **Archive Tables**
* During the Archiving process, some of the data is normalized and stored in a string of comma separated Record IDs.

## Deploy_Utilities Schedule

* The Archiving Process is performed by three programs executed from the **DEPLOY_UTILITIES** Schedule
* **ArchiveP.SMAOpConDeployClient.exe**
  * Used to perform an Archive of **Package Versions** no longer required in the ```deploy_package``` table
  * The process checks Schedules and Transformation Rules associated with the Package
  * If the Package is archived, any deployment records that reference the Package Record will also be archived
* **ArchiveS.SMAOpConDeployClient.exe**
  * Used to perform an Archive of **Schedule Versions** no longer required in the ```deploy_schedule``` table
  * If the schedule is archived, any deployment records that reference the Schedule Record will also be archived
* **ArchiveT.SMAOpConDeployClient.exe**
  * Used to perform an Archive of **Transformation Rule Versions** no longer required in the ```deploy_transformation_rule``` table