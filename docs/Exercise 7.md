---
sidebar_label: 'Exercise 7'
---

## Deploy Exercise 7: Script Deploy Function

### Objective

Use the Script Deploy Function.

### Summary

Validate that the scripts inside of Deploy do **NOT** exist the OpCon-QA environment by using Enterprise Manager. Deploy the scripts to the ```OpCon-QA``` Server. Validate that the scripts inside of Deploy **DO** exist the OpCon-QA environment by using Enterprise Manager.

### Instructions

#### Validate Script Existence in EM

1. Open the Enterprise Manager using the profile for the ```OpCon-QA``` Environment
  * **Username:** ```ocadm```
  * **Password:** ```opconxps```
2. Go to the **Scripts** section and open the **Script Repository** window
3. Validate that the **Create_Folder** and **SetThreshold** Scripts do **NOT** exist
  * If they do exist, double click on each to open the **Versions** window and make a note of how many versions exist for each
4. Close the **Script Repository** tab.
5. **Minimize** Enterprise Manager.

#### Deploy the Scripts

6. Back in Deploy, go to the **Scripts** section and click on the **Deploy** option
7. Click **Refresh** to list all the scripts that are in Deploy
8. You will notice the scripts are listed in the top half of the screen
9. Expand the **Create_Folder** by clicking the ```>``` next to the script to show the available versions
10. Right-Click the most recent version and select **View Script Content**
11. Click **Close**
12. Now Double-Click that version and note that it appears in the lower half of the screen
13. Now expand the ```SetThreshold``` script that is in the top half of the screen
14. Click on the latest version of that Script and then click the **Down Arrow** to move the version to the lower half of the screen
15. Now click the **Double Up Arrow** and notice that all the selected versions disappear from the bottom half of the screen
16. Now click the **Double Down Arrow** and this will return both script's **Version 1** to bottom half of the screen
17. Click the **Next** button
18. On the **Select a Server** screen, select the ```OpCon-QA``` server from dropdown
19. Click the **Next** button to open the **Script Deployment** screen

:::note

* You should be able to see the ```OpCon-QA``` server listed under Server although this will be greyed out. 
* You should also see the two scripts ```Create_Folder``` and ```SetThreshold``` under **Scripts**, these will also be greyed out

:::

20. Now click the **Finish** button
21. In the popup, click the **OK** button to execute the Deployment of the scripts
22. In the **Review Result of Deployment** screen, you should see that two scripts have been Deployed with ```0``` failures and the Status column should say **SUCCESS**
23. Click **Close** 
24. Stay logged in as **az-win10-deploy\SMAUSER** for the next exercise.

#### Validate Script Existence in EM

25. Open Enterprise Manager from the Toolbar
26. Go to the **Scripts** section and open the **Script Repository** window2
27. Validate that the **Create_Folder** and **SetThreshold** Scripts **DO** exist
  * Double click on each to open the **Versions** window and make a note of how many versions exist for each, it should match the number from the beginning of the exercise.
28. Close the **Script Repository** tab.
29. Close Enterprise Manager

:::info Video Walkthrough

[Deploy Scripts](../static/imgdeploy/Deploy_ScriptDeployment.mp4)

:::