---
sidebar_label: 'Deploy Lab'
hide_title: 'false'
---

## Deploy Lab

##### Objective: 

At the start of the exercises from this training: 

* Two different Users were created for the Deploy environment 
    * During this **LAB**, a specific **User ID** previously created may be needed to perform certain functions
* **Congo Online Retail** Schedules created in the ```OpCon-Dev``` Environment were moved to the ```OpCon-QA``` Environment 

* As part of this **LAB**, various changes will be made to the ```OpCon-QA``` Environment 
    * These changes will be imported back into the **Deploy** database and deployed to the ```OpCon-Prod``` Environment 
    * During the deployment process, further changes will be made via a Transformation Rule and Auto*Build options for **Production**

 :::warning note

 The ```OpCon-Prod``` Environment utilizes the same machine as the ```BatchScheduleServer``` Environment - so when creating a Transformation Rule the notation should be:

 ```OpCon-QA``` ---> ```OpConBatchDB```   

:::

##### Lab Instructions: 

:::note note

Remember that in this ecosystem, the ```OpCon-Prod``` Environment in Enterprise Manager uses the same **Machine Name** as the ```BatchScheduleServer```, which is ```OpConBatchDB```

(So when a Transformation Rule is made, it should read as ```OpCon-QA``` ---> ```OpConBatchDB```)

:::


* Change the Jobs in the ```OpCon-QA``` environment using Enterprise Manager such that the  **Congo Inventory Reports** jobs: **Legos**, **Levis**, **Nerf**, **Nike**, **Smartphones** and **Xbox** all use the parameter ```-t25``` on the command line
    * Import the changed Schedule into the **Deploy** database so the newer Version can be deployed to the ```OpCon-Prod``` Environment

* Use a **Transformation Rule** to change all command lines with a parameter of ```-t25``` to ```-t20``` 
    * Jobs in the **Congo Inventory Reports** Schedules have this parameter

* Ensure that all the Windows Jobs on the **Congo Inventory Reports** Schedule have the Machine changed to ```OpCon-Prod```

* On the ```OpCon-Prod``` System, the Jobs in the **Congo Inventory Reports** Schedule may not start until ```7:00 AM``` 
    * Change the Jobs using Enterprise Manager 
    * Import the changed Schedule into the Deploy database so the newest Version can be deployed to the ```OpCon-Prod``` Environment

* Change the **AutoBuild Schedule Details** in the Deployment details so that the Schedule builds ```3 Days in Advance for 1 day```

* Once Deployed, use **Enterprise Manager** on the ```OpCon-Prod``` Environment to ensure all changes have been made as expected


<!--
<video width="320" height="240" controls>
  <source src="imgdeploy/Deploy_Lab.mp4" type="video/mp4"></source>
Your browser does not support the video tag.
</video>
-->