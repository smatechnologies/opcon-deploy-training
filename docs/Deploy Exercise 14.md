---
sidebar_label: 'Deploy Exercise 14'
hide_title: 'false'
---

## Deploy Exercise 14: Steps to Perform a Batch Deployment

### Objective

Using the **Administration User** Log in, Batch Deploy a Schedule and Verify the Results

* Batch Deploy the **Congo Inventory Management** Schedule to the ```OpCon-QA``` Server
  * Use the ```Dev-to-QA-Machines``` Transformation Rule
* Verify that the Jobs in the Schedule have the correct Machine assigned

### Instructions

#### This exercise will select a schedule to be deployed and set a batch deployment to run at a specific date and time

1.	Open the Deploy Client using the **Administration User**
2.	Go to the **Deployments** section and click on the **Deploy** link to open the **Select a Deployment Type** window
3.	Click on the **Schedule** button to open the **Select a Schedule to Deploy** window
4.	Select the Schedule ```Congo Inventory Management``` - Available Versions for that Schedule will appear in the bottom half of the screen
5.	Select the Latest Version available and click the **Next** button
6.	This will open the **Select a Server** screen
7.	Select the ```OpCon-QA``` Server from the **Select OpCon Server** dropdown list
8.	Click the **Next** button to advance to the **Select transformation Rules** screen
9.	Select the Latest Version of the ```Dev-to-QA-Machines``` Transformation Rule and move it to the lower half of the screen by Double-Clicking on it or by using the arrows between the screen halves
10.	Click the **Simulate** button and check the **Result of the Simulation** for errors
11.	Close the Result of the Simulation screen by clicking the **Close** button
12.	Click the Batch Deploy button to open the Additional information for Batch Deployment screen
13.	Select the **Date** and **Time** for the Deployment to run
:::caution Note
Use today's date (Not a future date) - Do Not enter a time (It will default to 00:00)
:::
14.	Enter the current user's **User Password** in the **Password** text box 
15.	Click the **OK** button to receive a selection confirmation - Click **OK** to proceed with Deployment
16.	A **Batch Deployment** popup will state **"The Schedule has been scheduled for batch deployment successfully”**  
17. Click the **OK** button to close the popup 
18.	Now repeat the steps **2** to **16** to Deploy the **Congo Payroll Payments** Schedule and the **Congo Inventory Reports** Schedule
19.	Using EM connect to the ```OpCon-QA``` Environment and verify that the Schedule Master record was updated for the **Congo Inventory Management** and the **Congo Payroll Payments** Schedules
20.	Now open the **Job Master** screen to view the jobs in the **Congo Inventory Management** Schedule 
21. Edit the Jobs in this Schedule and check that the Machine is correct, the Windows Jobs should be using the ```OpCon-QA``` Machine and the **Inventory Purchase Report** Job should be running on the Machine ```Susevm``` (These Machine Names should have been changed as part of the Transformation Rules)
22.	Once the check is completed completed, close Enterprise Manager

:::info Video Walkthrough

[Batch Deployment](../static/imgdeploy/Deploy_BatchDeployment.mp4)

:::