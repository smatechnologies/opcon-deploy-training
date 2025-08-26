---
sidebar_label: 'Deploy Lab'
---

## Deploy Lab

### Objective

Deploy schedules that have been changed in the OpCon-QA environment into Production.

### Summary

Using the **Administration User**, make modifications to the jobs in the **Congo Inventory Report** schedule to have a new value for the **-t parameter** in the QA Environment and **import** the schedule into Deploy. Then deploy the schedule into **OpCon-Prod** using a **Transformation Rule** that will **update** the command line, start time, and machine name of the jobs.

:::note

The **OpCon-Prod Environment** in Enterprise Manager uses the same **Machine Name** as the ```BatchScheduleServer```, which is ```OpConBatchDB```

(So when a Transformation Rule is made, it should read as ```OpCon-QA``` &rarr; ```OpConBatchDB```)

:::

### Lab Instructions

* In the ```OpCon-QA``` environment using Enterprise Manager modify the **Congo Inventory Reports** jobs: **Legos**, **Levis**, **Nerf**, **Nike**, **Smartphones** and **Xbox** to use the parameter ```-t25``` in the command line
  * Import the changed Schedule into the **Deploy** database so the newer Version can be deployed to the ```OpCon-Prod```
* Use a **Transformation Rule** to change:
  * The command lines with a parameter of ```-t25``` to ```-t20``` 
    * Jobs in the **Congo Inventory Reports** Schedules have this parameter
  * The windows machine name from ```OpCon-QA``` to ```OpConBatchDB```
  * The schedule starts at **7:00 AM**
* Ensure that Auto Build is set to ```3 Days in Advance for 1 day``` when it is deployed
* Once the Deploy is successful, use **Enterprise Manager** to connect to the ```OpCon-Prod``` environment to ensure all changes have been made as expected
  * **User Name:** ```ocadm``` 
  * **Password:** ```opconxps```

:::info Video Walkthrough

[Comprehensive Lab](../static/imgdeploy/Deploy_Lab.mp4)

:::