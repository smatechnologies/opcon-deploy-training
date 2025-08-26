---
sidebar_label: 'Exercise 11'
---

## Deploy Exercise 11: Transformation Rules

### Objective

To create a Transformation Rule

### Summary

Use the **Windows Authentication** login to Create Transformation Rules in Deploy that will modify the **Machines** when a deployment occurs.

### Instructions

1.	On the Login screen, check **Use Windows Authentication** 
2.  Click **Login**
3. Click on the **Create/Edit** option in the **Transformation Rules** section
4.	Click **Add**
5.	In the **Name** field, enter ```Dev-to-QA-Machines```
6.	In the **Description** field, enter ```Will convert the Machines Names in the Dev Env to correct names for the QA Env```
7.	In the **List of Transformation** section, click the **green +** button
8. In the **Create or Edit a Transformation** screen,
  * In the **Tag ID** dropdown, select **Job: Machine Name**
  * In the **Current Value** textbox enter ```OpCon-Dev```
  * In the **New Value** text box enter ```OpCon-QA```
  * Click the **Save** button
9.	Repeat the Step 8 to add a rule to change the **Susevm1** machine name to **Susevm**
10.	Click **Save**
11.	Click **Close**
12. Stay logged in as **az-win10-deploy\SMAUSER** for the next exercise.



:::info Video Walkthrough

[Create Transformation Rules](../static/imgdeploy/Deploy_CreateTransformationRules.mp4)

:::