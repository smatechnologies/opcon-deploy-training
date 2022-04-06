---
sidebar_label: 'Deploy Exercise 4'
hide_title: 'false'
---

## Deploy Exercise 4: Steps To Check Audit Records

##### Objective:

Use the Windows Authentication User to Check Audit records for:

- Windows Authentication (```az-win10-deploy\SMAUSER```) User 
- ```DeployTeamLeader``` User

### Instructions

1.	Open the **Deploy Client** and check **Use Windows Authentication** to log in in with the ```az-win10-deploy\SMAUSER``` login
2.	Go to the **Administration** section, notice that only Audits listed can be seen
3.	Click **Audits** to open the **View Audit Messages** screen
4.	From the Category dropdown list select Server
5.	From the **User** dropdown list select the User ```az-win10-deploy\SMAUSER```
6.	Select appropriate **From** and **To** Dates
7.	Click **Apply**
8.	Notice that nothing appears in the right of the screen, as changes were not made to the Server information using this User login
9.	Now change the selection in the **User** dropdown to select the User used to create the Server records
10.	Click **Apply**
11.	The **Audit information** for Server Record Creation should appear in the right-hand pane of the screen
12.	When finished checking the Audit information, click the **Close** button to close out the screen

<video width="320" height="240" controls>
  <source src="imgdeploy/Deploy_CheckAuditRecords.mp4" type="video/mp4"></source>
Your browser does not support the video tag.
</video>