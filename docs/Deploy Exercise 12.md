---
sidebar_label: 'Deploy Exercise 12'
hide_title: 'false'
---

## Deploy Exercise 12: Steps to Browse a Transformation Rule

### Objective

Still Using the ```Windows Authentication``` Login:

- Use the **Browse** link under **Transformation Rules**
  - Open **Browse and Filter Transformation Rules**

- Create a new ```Transformation``` by Editing the ```Dev-to-QA-Machines``` Transformation Rule
  - Create a new ```Tag ID``` using **Resource Name**
  - Give a **Current Value** of ```Electronics```
  - Give a **New Value** of ```Electronics-QA```

- Now Browse ```Version 2``` of the ```Dev-to-QA-Machines``` **JSON** file  
  - Verify that all three Definitions exist in the new **Transformation Rule**

### Instructions

#### Browse the Transformation Rule created in the previous exercise and add one more Rule to the list of Transformations

1.	Go to the **Transformation Rules** section and click on the **Browse** link - This will open the **Browse and Filter Transformation Rules** screen *(You may need to click the REFRESH button to view the Transformation Rules)*
2.	Take note of the **Name** text box as this can be used to filter the Transformation Rules when there are many Rules in the database
3.	Now expand the ```Dev-to-QA-Machines``` Transformation Rule by clicking the ```>```
4.	Right-Click the ```Version 1``` of the Transformation Rule and the **Edit a Transformation Rule** screen will open
5.	Click the **green** ```+``` button to open the **Create or Edit a Transformation** screen
6.	From the **Tag ID** dropdown list select **Resource Name**
7.	In the **Current Value** text box, enter ```Electronics```
8.	In the **New Value** text box, enter ```Electronics-QA```
9.	Click the **Save** button to save this new Transformation pattern
10.	Click the **Save** button to save this change to the Transformation Rule
11.	Click **OK** to the popup message that says a new Version of the Transformation Rule has been saved
12.	Check that this new Version is visible in the **Browse and Filter Transformation Rules** screen *(You may need to click the REFRESH button to view the Transformation Rules)*
13.	Now right-Click ```Version 2``` of the ```Dev-to-QA-Machines ``` Transformation Rule and select **View Definition**. This will open the Definition of ```[Dev-to-QA-Machines] ``` screen
14.	**Machine Names** should be clearly visible as they will be created when the Transformation Rule is used, as should the new Value that will be used for the **Resource Name**
15.	When you have finished viewing the **JSON** format of the Transformation Rule, close the window by clicking the **Close** button
16.	Close the **Browse and Filter Transformation Rules** screen by clicking the **Close** button

:::tip [Walkthrough Video - Exercise 12](../static/imgdeploy/Deploy_BrowseTransformationRules.mp4)

:::