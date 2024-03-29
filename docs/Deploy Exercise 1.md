---
sidebar_label: 'Deploy Exercise 1'
hide_title: 'false'
---

## Deploy Exercise 1: Create User IDs

### Objective

Create two Users within the Deploy Client

- Create a User that utilizes Windows Authentication and a User that does NOT utilize Windows Authentication

### Instructions

#### Create A Windows Authentication User 

1.	Open the Deploy client and log in using the **User Name** ```admin``` and with a **Password** of ```admin```
2.	Under the **Administration** section click on **Users** to open the **User Management** screen
3.	Click the **Add** button
4.	In the **User Name** text box, enter ```az-win10-deploy\SMAUSER```
:::note Note
The Password Field will be empty for Windows Authentication Logins
:::
5.	In the **Description** text box, enter your name and surname 
6.	From the **Role** dropdown list select **Non-Production**
7.	Check the **View Audit Messages** checkbox is checked
8.	In the **OpCon User Name** text box, enter ```ocadm```
9.	In the **OpCon Password** text box, enter the password of ```opconxps```
10.	Click the **Save** button

#### Create A User That Does Not Use Windows Authentication

1.	Now click the **Add** button again
2.	In the **User Name** text box, enter ```DeployTeamLeader```
3.	In the **Password** text box, enter ```deployadmin```
4.	In the **Description** text box, enter the name and surname of the Deployment Team Leader
5.	From the **Role** dropdown list select ```Administration```
6.	In the **OpCon User Name** text box, enter ```ocadm```
7.	In the **OpCon Password** text box, enter the password of ```opconxps```
8.	Click the **Save** button
9.	Click the **Close** button
10.	Log out of the **Deploy client**

:::tip [Walkthrough Video - Exercise 1](../static/imgdeploy/Deploy_CreateUserIDs.mp4)

:::