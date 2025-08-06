---
sidebar_label: 'Deploy Terminology'
hide_title: 'false'
---

## Deploy Terminology

* **Import:** The process of extracting a Schedule Definition from the source OpCon Environment
* **Deploy:** The process of selecting a Schedule Definition from the Central Repository and inserting it into the target OpCon Environment
* **Package:** A group of Schedule definitions that can be deployed as a single unit to an OpCon system
  * Once a Schedule definition is included in a Package, it cannot be deployed as a single entity to the Production system
  * A schedule can only belong to a single package per OpCon system
* **Schedules:** The Schedules function support the capabilities required to import and view Schedule definitions
* **Transformation Rules:** Can be used to transform a Schedule definition during Deployment to match the specific requirements of the target OpCon system
* **Simulation:** Performs a Deployment check without updating the Schedule Definition on the target OpCon System
* **Rollback:** Performs a restore of a Schedule Definition from the backup taken during the Deploy process
* **Batch Schedule Server:** The Batch Schedule Server is used to schedule Batch deployments at the requested date and time, archive tasks, and perform database backups.
  * One of the OpCon systems participating in the Deploy environment should be designated as the Batch Schedule Server. 
* **BATCH_DEPLOY Schedule:** This schedule must be available on the Batch Schedule Server
  * If it doesn't exist on the Batch Schedule Server, it will be Deployed at the time of the first scheduled deployment.
* **Delete:** Removes a Package or Schedule from the selected OpCon System