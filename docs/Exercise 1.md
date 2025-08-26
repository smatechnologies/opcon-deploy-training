---
sidebar_label: 'Exercise 1'
---

## Exercise 1: Deploy Users

### Objective

Create new User Accounts.

### Summary

Using the Admin User, you will create two new users, an **Administrator User** and a **Non-Production User**. The **Administrator** will have a **password assigned** to it while the **Non-Production user** will utilize **Windows Authentication**.

### Instructions

#### Create A Windows Authentication User 

1.	Open the Deploy client and log in using
  * **User Name:** ```admin``` 
  * **Password:** ```admin```
2.	Under the **Administration** section click on **Users** to open the **User Management** screen
3.	Click the **Add** button
4.	In the **User Name** text box, enter ```az-win10-deploy\SMAUSER```

:::note Note

The Password Field will remain empty when creating user that utilize Windows Authentication.

:::

5.	In the **Description** text box, enter your name and surname 
6.	From the **Role** dropdown list select **Non-Production**
7.	Verify the **View Audit Messages** checkbox is checked
8.	In the **OpCon User Name** text box, enter ```ocadm```
9.	In the **OpCon Password** text box, enter the password of ```opconxps```
10.	Click the **Save** button

#### Create A User That Does Not Use Windows Authentication

11.	Now click the **Add** button again
12.	In the **User Name** text box, enter ```DeployTeamLeader```
13.	In the **Password** text box, enter ```deployadmin```
14.	In the **Description** text box, enter ```Deploy Team Leader```
15.	From the **Role** dropdown list select ```Administration```
16.	In the **OpCon User Name** text box, enter ```ocadm```
17.	In the **OpCon Password** text box, enter the password of ```opconxps```
18.	Click the **Save** button
19.	Click the **Close** button
20.	Log out of the **Deploy client**

:::info Video Walkthrough

[Create User IDs](../static/imgdeploy/Deploy_CreateUserIDs.mp4)

:::