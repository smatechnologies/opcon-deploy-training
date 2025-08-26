---
sidebar_label: 'Exercise 4'
---

## Deploy Exercise 4: Deploy Audit

### Objective

Use Audit to check Audit Records

### Summary

Use the Windows Authentication User check Audit for any Server Records created by either the **Windows Authentication user** or the **Administrative User** user for today's date.

### Instructions

1.	On the Login screen, check **Use Windows Authentication** 
2.  Click **Login**
3.	Go to the **Administration** section

:::note

Notice that only Audits listed can be seen as this user is NOT an Administrator.

:::

4.	Click **Audits** to open the **View Audit Messages** screen
5.	From the Category dropdown list select Server
6.	From the **User** dropdown list select the User ```az-win10-deploy\SMAUSER```
7.	Select today's date for the **From** and **To** Date fields.
8.	Click **Apply**

:::note

Notice that nothing appears in the right of the screen, as changes were not made to the Server section using the Windows Auth user

:::

9.	Now change the selection in the **User** dropdown to select the **DeployTeamLeader** user
10.	Click **Apply**
11.	The **Audit information** for Server Record Creation should appear in the right-hand pane of the screen

:::note

You should see entries from where the Servers were created by this user in a previous exercise.

:::

12. Stay logged in as **az-win10-deploy\SMAUSER** for the next exercise.

:::info Video Walkthrough

[Check Audit Records](../static/imgdeploy/Deploy_CheckAuditRecords.mp4)

:::