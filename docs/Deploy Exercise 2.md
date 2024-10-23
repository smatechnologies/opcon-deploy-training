---
sidebar_label: 'Deploy Exercise 2'
hide_title: 'false'
---

## Deploy Exercise 2: Steps To Create Servers In The OpCon environment

### Objective

Create Four Server Connections Within the Deploy Client

- Create the Following Server Connections:
  - Quality Assurance (OpCon-QA)
  - Development (OpCon-Dev)
  - Production (OpCon-Prod)
  - Batch Schedule Server (BatchScheduleServer)

### Instructions

#### Create the server record for the Quality Assurance server in our OpCon environment

1.	Open the Deploy client and log in in with the User you just created that had **Administration Privileges**
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
14.	If the Server Connection was **not successful** review the instructions or ask the Trainer for assistance

#### Create the server record for the Development server in our OpCon environment

1.	Click the **Add** button
2.	In the **Server Name** text box, enter ```OpCon-Dev```
3.	From the **Server Type** dropdown list select **Development**
4.	Check the checkbox that **Allow Transformation Rules** has been selected
5.	In the **Server Address** text box add the server IP address of ```az-win10-deploy```
6.	In the **Server Port** text box enter the port number used by Deploy which is ```9070```
7.	Check that the checkbox for **Using TLS** is selected
8.	In the **OpCon API Port** text box, enter the **OpCon API Port Number** which is ```700```
9. Check that the checkbox for **Using TLS** is selected
10.	Click the **Test Server Connection** button
11.	If the server connection was **successful** click **Save** 
12.	If the server connection was **not successful** review the instructions or ask the Trainer for assistance

#### Create the server record for the Production server in our OpCon environment

1.	Click the **Add** button
2.	In the **Server name** text box, enter ```OpCon-Prod```
3.	From the **Server Type** dropdown list select **Production**
4.	Check the checkbox that **Allow Transformation Rules** has been selected
5.	In the **Server Address** text box add the server IP address of ```az-win10-deploy```
6.	In the **Server Port** text box enter the port number used by Deploy which is ```9011```
7.	Check that the checkbox for **Using TLS** is selected
8.	In the **OpCon API Port** text box, enter the **OpCon API Port Number** which is ```443```
9. Check that the checkbox for **Using TLS** is selected
10.	Click the **Test Server Connection** button
11.	If the server connection was **successful** click Save
12.	If the server connection was **not successful** review the instructions or ask the Trainer for assistance

:::note

The port information for BatchScheduleServer will be the same as the OpCon-Prod Server

:::

#### Create the server record for the BatchScheduleServer in our OpCon environment

1. Click the **Add** button
2. In the **Server name** text box, enter ```BatchScheduleServer```
3. From the **Server Type** dropdown list select **Production**
4. Check the checkbox that **Allow Transformation Rules** has been selected
5. In the **Server Address** text box add the server ```az-win10-deploy```
6. In the **Server Port** text box enter the port number used by Deploy which is ```9011```
7. Check that the checkbox for **Using TLS** is selected
8. In the **OpCon API Port** text box, enter the **OpCon API Port Number** which is ```443```
9. Check that the checkbox for **Using TLS** is selected
10. Click the **Test Server Connection** button
11. If the server connections was **successful** click **Save**
12. If the server connection was **not successful** review the instructions or ask the Trainer for assistance
<!--
:::tip [Walkthrough Video - Exercise 2](../static/imgdeploy/Deploy_CreateServers.mp4)

:::
-->