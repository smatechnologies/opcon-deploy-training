---
sidebar_label: 'Exercise 13'
---

## Deploy Exercise 13: Steps to Deploy a Package

### Objective

Deploy a Package

### Summary

Use the Deploy function to deploy a Package to the **OpCon-QA Environment** using the **Administration User**. Then verify the deployment results by utilizing Enterprise Manager.

### Instructions

#### Deploy a Package

1.  Open the Deploy Client using the **Administration User**
  * **User:** ```DeployTeamLeader```
  * **PWD:** ```deployadmin```
2.  In the **Deployments** section, click the **Deploy** option
3.  In the **Select a Deployment Type** window, click the **Package** button 
4.  In the **Select a Package to Deploy** window, click **Refresh**
5.  In the **Package List** section, select the **Congo HR Package**
6.  In the **Version** section, select **latest version** of the **Congo HR Package**
7.  Click **Next**
8.  In the **Select a Server** screen, select the ```OpCon-QA``` from the dropdown
9.  Click **Next** 
10. In the the **Select Transformation Rules** screen, click **Refresh**
11. Expand the **Dev-to-QA-Machines** rule using the **>**
12. Double click the **Latest Version** of the rule to move it to the bottom of the screen
13. Click **Next** to see how the **transformation** will be applied during **Deployment**
14. Click **Simulate**
15. Review **Result of Simulation** screen for possible errors

:::note

_If there are warnings or errors this will be indicated in red at the top of the screen_

:::

16. Click **Close** 
17. Click **Deploy** 
18. Click **OK** on the popup window confirming the Package Name to be Deployed
19. Stay logged in as the **DeployTeamLeader** for the next exercise

#### Validate Deployment in Enterprise Manager

20. Log into **OpCon-QA Environment** with **Enterprise Manager**
  * **User:** ```ocadm```
  * **PWD:** ```opconxps```
21. In the **Navigation Panel** double-click **Schedule Master** 
22. Select the **HR Import** schedule from the dropdown
23. Open the **Deploy Info** tab and review the information

:::note

* You should see the following:
  * Version: #
  * Package: PackageName : version #
  * Description: 
  * Record Id: #
  * Deployed: DeployTeamLeader (yyyy-mm-dd hh:mm:ss)

:::

24. Close the **Schedule Master** tab
25. In the **Navigation Panel** double-click **Job Master** 
26. In the **Schedule** dropdown, select the **HR Import**
27. In the **Job** dropdown, select **Create HR Files**
28. Validate that the **Primary Machine** dropdown shows ***OpCon-QA**.
29. Close the **Job Master** tab
20. Minimize Enterprise Manager 

:::info Video Walkthrough

[Deploy a Package](../static/imgdeploy/Deploy_DeployPackage.mp4)

:::