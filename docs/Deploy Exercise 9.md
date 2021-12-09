---
sidebar_label: 'Deploy Exercise 9'
hide_title: 'false'
---

## Deploy Exercise 9: Steps to View a Schedule Stored in Deploy

##### Objective: 

Use the ```Windows Authentication User``` to Browse Imported Schedules in the Deploy Client

- Open the JSON Definition File for the **HR Import** Schedule
- Search for the word **name** within the file
- Choose one for keyword to search for practice

<div>
<video width="320" height="240" controls>
  <source src="imgdeploy/Deploy_BrowseSchedules.mp4" type="video/mp4"></source>
Your browser does not support the video tag.
</video>
</div>

<details>

<summary>Click for Step-By-Step Instructions</summary>

#### Test the Schedule Browse Function by Browsing a Recently Imported Schedule

1.  Open the Deploy Client and check Use Windows Authentication to log in in with the ```az-win10-deploy\SMAUSER``` login
2.	Go to the **Schedules** section and click on the **Browse** link - This will open the **Browse and Filter Schedules Imported** screen.
3.  Note the **Name** text box that can be used to filter the list of Schedules
4.	Now click the ```>``` next to the **HR Import** Schedule to expand the list of Versions of this Schedule that are available
5.	Right-Click the latest Version of the **HR Import** Schedule and select **View Definition**
6.	The Definition of **[HR Import]** screen will open to show the **JSON** format of all the information of the Schedule
7.	Type name in the filter text box and press Enter - Note the first occurrence of name will be highlighted in blue
8.  At the right end of the text box, you will note 1 of x and some arrows that will help you navigate through the document according to the filter you have entered
9.	Now put a new selection in the filter text box and test the filter action for yourself
10.	When you have finished your activities click the **Close** button to close this window
11.	Now click the **Close** button to close out the **Browse and Filter Schedules Imported** screen

</details>