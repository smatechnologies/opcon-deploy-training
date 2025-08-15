---
sidebar_label: 'Exercise 4'
---

## Deploy Exercise 4: Steps To Check Audit Records

### Objective

Use Audit to check Audit Records

### Summary

Using the Windows Authentication User, ```az-win10-deploy\SMAUSER```, to check Audit for any Server Records created by either the **Windows Authentication user** or the **DeployTeamLeader** user for today's date.

### Instructions

1.	Open the **Deploy Client** and check **Use Windows Authentication** 
  * **User:** ```az-win10-deploy\SMAUSER```
2.	Go to the **Administration** section

:::note

Notice that only Audits listed can be seen as this user is NOT an Administrator.

:::

3.	Click **Audits** to open the **View Audit Messages** screen
4.	From the Category dropdown list select Server
5.	From the **User** dropdown list select the User ```az-win10-deploy\SMAUSER```
6.	Select today's date for the **From** and **To** Date fields.
7.	Click **Apply**

:::note

Notice that nothing appears in the right of the screen, as changes were not made to the Server section using the Windows Auth user

:::

8.	Now change the selection in the **User** dropdown to select the **DeployTeamLead** user
9.	Click **Apply**
10.	The **Audit information** for Server Record Creation should appear in the right-hand pane of the screen

:::note

You should see entries from where the Servers were created by this user in a previous exercise.

:::

:::info Video Walkthrough

[Check Audit Records](../static/imgdeploy/Deploy_CheckAuditRecords.mp4)

:::