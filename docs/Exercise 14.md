---
sidebar_label: 'Exercise 14'
---

## Deploy Exercise 14: Steps to Perform a Batch Deployment

### Objective

Schedule a Batch Deployment

### Summary

Using the **Administration User** schedule a batch deployment for multiple schedules. Then verify the deployment results by utilizing Enterprise Manager.

### Instructions

1.	In **Deploy**, in the **Deployments** section, click **Deploy** 
2. In the **Select a Deployment Type** window, click on the **Schedule** button
3. In the **Select a Schedule to Deploy** window, click **Refresh** 
4. In the **Schedule List**, select **Congo Inventory Management**
5. In the **Version** section, select the **latest version**
6.	Click **Next**
7.	In the **Select a Server** screen, select **OpCon-QA** from the dropdown
8.	Click **Next** 
9. In the **Select transformation Rules** screen, Click **Refresh**
10. Expand the **Dev-to-QA-Machines** rule using the **>**
11. Double click the **Latest Version** of the rule to move it to the bottom of the screen
12. Click **Next** to see how the **transformation** will be applied during **Deployment**
13.	Click **Simulate**
14. Check the **Result of the Simulation** for any errors
15.	Click **Close**
16.	Click **Batch Deploy**
17. In the **Additional information for Batch Deployment** popup, set the **Date** and **Time** for the Deployment to run
  * Use **today's date** and leave the **time at 00:00**
18. Enter in the **DeployTeamLeader** password, ```deployadmin```
19. Click **OK**
20. Confirm the deployment by clicking **OK**
21.	A **Batch Deployment** popup will state **"The Schedule has been scheduled for batch deployment successfully”**  
22. Click **OK** 
23.	Repeat **Steps 2-22** to Deploy the **Congo Payroll Payments** and the **Congo Inventory Reports** Schedules
24. Stay logged in as **aDeployTeamLeader** for the next exercise.


#### Validate Deployment in Enterprise Manager

25. Log into **OpCon-QA Environment** with **Enterprise Manager**
  * **User:** ```ocadm```
  * **PWD:** ```opconxps```
26. In the **Navigation Panel** double-click **Schedule Master** 
27. Select the **Congo Inventory Management** schedule from the dropdown
28. Open the **Deploy Info** tab and review the information

:::note

* You should see the following:
  * Version: #
  * Description: 
  * Record Id: #
  * Deployed: DeployTeamLeader (yyyy-mm-dd hh:mm:ss)

:::

29. Close the **Schedule Master** tab
30. In the **Navigation Panel** double-click **Job Master** 
31. In the **Schedule** dropdown, select the **Congo Inventory Management**
32. In the **Job** dropdown, select **Legos**
33. Validate that the **Primary Machine** dropdown shows ***OpCon-QA**.
34. In the **Job** dropdown, select **Inventory Purchase Report**
35. Validate that the **Primary Machine** dropdown shows ***Susevm**.
36. Close the **Job Master** tab
37. Close out of Enterprise Manager 

:::info Video Walkthrough

[Batch Deployment](../static/imgdeploy/Deploy_BatchDeployment.mp4) 

:::