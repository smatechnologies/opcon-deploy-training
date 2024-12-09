---
sidebar_label: 'Deploy Exercise 7'
hide_title: 'false'
---

## Deploy Exercise 7: Steps to Perform Script Deployment

### Objective

Deploy Two Scripts (```Create_Folder``` and ```SetThreshold```) to the ```OpCon-QA``` Server

- Verify first that two Scripts do not exist in the ```OpCon-QA``` Enterprise Manager profile
- After Deployment, Verify that the two Scripts are now visible in the ```OpCon-QA``` Enterprise Manager profile

### Instructions

#### Check the Scripts on the OpCon-Dev Environment and Deploy the Scripts to that Environment

1.	Open the Enterprise Manager using the profile for the ```OpCon-QA``` Environment
2.	Go to the **Scripts** section and open the **Script Repository** window
3.	Check if the ```Create_Folder``` and the ```SetThreshold``` Scripts exist
4.	If they do exist, double click on each in turn to open the **Versions** window and make a note of how many versions exist for each
5.	Now open the Deploy Client.
6.	Go to the **Scripts** section and click on the Deploy link - This should open the **Select Scripts** window
7.	You will notice the ```Create_Folder``` script listed in the top half of the screen - Click the ```>``` next to ```Create_Folder``` to show the available versions *(You may need to click the REFRESH button to view the Scripts)*
8.	Right-Click the most recent version and select **View Script Content** - Once you have checked the contents of the Script click the **Close** button
9.	Now Double-Click that version and note that it appears in the lower half of the screen
10.	Now expand the versions below the ```SetThreshold``` Script that is in the top half of the screen
11.	Click on the latest version of that Script and then click the **Down Arrow** between the two screen halves - Notice that version of the ```SetThreshold``` Script is pushed to the bottom half of the screen
12.	Now click the double up arrow and notice that all the selected versions disappear from the bottom half of the screen
13.	Now click the **Double Down Arrow** and this will return both the ```Create_Folder``` Script and the ```SetThreshold``` Script to bottom half of the screen
14.	Click the **Next** button, this will open the **Select a Server** screen
15.	Select the ```OpCon-QA``` server from the **Select OpCon Server** dropdown list
16.	Click the **Next** button and you will notice the **Script Deployment** screen will open
17.	You should be able to see the ```OpCon-QA``` server listed under Server although this will be greyed out
18.	You should also see the two scripts ```Create_Folder``` and ```SetThreshold``` under **Scripts**, these will also be greyed out
19.	Now click the **Finish** button
20.	A popup message will be displayed alerting that **2 Scripts Will Be Deployed on the Server ```OpCon-QA```. Do you want to proceed with Deployment?** Click the **OK** button to execute the Deployment
21.	Once the Deployment is finished a window will open called **Review Result of Deployment**. It should indicate that 2 Scripts have been Deployed with ```0``` failed. The Status column should indicate **SUCCESS**
22.	Once you have checked, you can close this action out by clicking the **Close** button
23.	Open Enterprise Manager using a profile that opens the ```OpCon-QA``` Environment 
24. Go to the **Scripts Repository** and check for the expected Scripts and Version in the Repository

<video width="320" height="240" controls>
  <source src="imgdeploy/Deploy_ScriptDeployment.mp4" type="video/mp4"></source>
Your browser does not support the video tag.
</video>