---
sidebar_label: 'Exercise 2'
---

## Deploy Exercise 2: Deploy Servers

### Objective

Define Servers within Deploy.

### Summary

Using the Deploy UI, define four servers: a **Quality Assurance** server, a **Development** server, a **Production** server, and a **Batch Schedule Server**. Each will have a **unique name** and **ports** in order for Deploy to establish connections to each of the OpCon environments they represent.

### Instructions

:::note

If any connection test is **unsuccessful**, please let the instructor know.

:::

#### Define the Quality Assurance Server

1.	Open the Deploy client and log in in with the User you just created that had **Administration Privileges**
  * **User:** ```DeployTeamLeader```
  * **PWD:** ```deployadmin```
2.	Under the **Administration** section click on Servers to open the **Server Management** screen
3.	Click the **Add** button
4.	In the **Server Name** text box, enter ```OpCon-QA```
5.	From the **Server Type** dropdown list select **Quality Assurance**
6.	Check the checkbox that **Allow Transformation Rules** has been selected
7.	In the **Server Address** text box add the server address of ```az-win10-deploy```
8.	In the **Server Port** text box enter the port number used by Deploy which is ```9060```
9.	Check that the checkbox for **Using TLS** is selected
10.	In the **OpCon API Port** text box, enter the **OpCon API Port Number** which is ```600```
11. Check that the checkbox for **Using TLS** is selected
12.	Click the **Test Server Connection** button
13.	If the Server Connection was **successful** click **Save**

#### Define the Development Server

14.	Click the **Add** button
15.	In the **Server Name** text box, enter ```OpCon-Dev```
16.	From the **Server Type** dropdown list select **Development**
17.	Check the checkbox that **Allow Transformation Rules** has been selected
18.	In the **Server Address** text box add the server IP address of ```az-win10-deploy```
19.	In the **Server Port** text box enter the port number used by Deploy which is ```9070```
20.	Check that the checkbox for **Using TLS** is selected
21.	In the **OpCon API Port** text box, enter the **OpCon API Port Number** which is ```700```
22. Check that the checkbox for **Using TLS** is selected
23.	Click the **Test Server Connection** button
24.	If the server connection was **successful** click **Save** 

#### Define the Production Server

25.	Click the **Add** button
26.	In the **Server name** text box, enter ```OpCon-Prod```
27.	From the **Server Type** dropdown list select **Production**
28.	Check the checkbox that **Allow Transformation Rules** has been selected
29.	In the **Server Address** text box add the server IP address of ```az-win10-deploy```
30.	In the **Server Port** text box enter the port number used by Deploy which is ```9011```
31.	Check that the checkbox for **Using TLS** is selected
32.	In the **OpCon API Port** text box, enter the **OpCon API Port Number** which is ```443```
33. Check that the checkbox for **Using TLS** is selected
34.	Click the **Test Server Connection** button
35.	If the server connection was **successful** click Save

:::info

The port information for BatchScheduleServer will be the same as the OpCon-Prod Server

:::

#### Define the BatchScheduleServer Server

36. Click the **Add** button
37. In the **Server name** text box, enter ```BatchScheduleServer```
38. From the **Server Type** dropdown list select **Production**
39. Check the checkbox that **Allow Transformation Rules** has been selected
40. In the **Server Address** text box add the server ```az-win10-deploy```
41. In the **Server Port** text box enter the port number used by Deploy which is ```9011```
42. Check that the checkbox for **Using TLS** is selected
43. In the **OpCon API Port** text box, enter the **OpCon API Port Number** which is ```443```
44. Check that the checkbox for **Using TLS** is selected
45. Click the **Test Server Connection** button
46. If the server connections was **successful** click **Save**
47. Click **Close**.
48. Stay logged in as **DeployTeamLeader** for the next exercise.

:::info Video Walkthrough

[Create Servers](../static/imgdeploy/Deploy_CreateServers.mp4)

:::