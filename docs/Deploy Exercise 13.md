---
sidebar_label: 'Deploy Exercise 13'
hide_title: 'false'
---

## Deploy Exercise 13: Steps to Deploy a Package

### Objective

Deploy a Package to the ```OpCon-QA``` Environment with the **Adminstration User**

- Deploy the ```Congo HR Package``` to the ```OpCon-QA``` Server
- Include the ```Dev-to-QA-Machines``` Transformation Rule 
- Check the Simulation of the Deployment
- Complete the Deployment 

Log In to Enterprise Manager with the ```OpCon-QA``` Environment to: 

- Check that the Deployment occurred 
- Check that the Transformation Rules were applied

### Instructions

1.	Open the Deploy Client using the **Administration User**
2.	Go to **Deployments** and click the **Deploy** link to open the **Select a Deployment Type** window
3.	Click on the **Package** button to open the **Select a Package to Deploy** window *(You may need to click the REFRESH button to view the Packages)*
4.	Click on the Package you created previously - ```Congo HR Package``` - it should be visible in the **Package List**
5.	This will display the Versions of this Package in the lower half of the screen
6. Select the **Latest Version** and click the **Next** button - This will open the **Select a Server** screen
7.	From the **Select OpCon Server** dropdown select the ```OpCon-QA``` Server
8.	Click the **Next** button to advance to the **Select Transformation Rules** screen
9.	Select the **Latest Version** of the ```Dev-to-QA-Machines``` Transformation Rule and move it to the lower half of the screen - This can be done by Double-Clicking or by using the arrows between the screen halves *(You may need to click the REFRESH button to view Transformation Rules)*
10.	Click the **Simulate** button - This will open the **Results of Simulation** screen, displays any warnings or errors 
:::note Note
_If there are warnings or errors this will be indicated in red at the top of the screen_
:::
11.	After checking for any possible errors, click the **Close** button to close the screen
12.	Click the **Deploy** button to Deploy the Package to the ```OpCon-QA``` Server
13.	A popup message will display confirming the Package Name to be Deployed and the Server on which it should be Deployed - If these details are correct, click the **OK** button
14.	Once the Deployment has completed, log in to EM with the ```OpCon-QA``` System
15.	Open the **Schedule Master** screen and select each of the Schedules from the Package in turn, ```HR Import``` and ```HR Import Processing``` 
16. Once you have a Schedule selected, open the **Deploy Info** tab and review the information - You should see the Version of the Schedule that was Deployed, as well as your User ID information
17.	Open the **Job Master** screen to view the jobs in the ```HR Import``` and ```HR Import Processing``` Schedules
18. Edit the Jobs in these Schedules and check that the Machine is correct - the Windows Jobs should be using the ```OpCon-QA``` Machine (These Machine Names should have been changed as part of the **Transformation Rules**)
