---
sidebar_label: 'Exercise 8'
---

## Deploy Exercise 8: Schedule Import Function

### Objective

Import Schedules into Deploy

### Summary

Using the **Import** option in the **Schedule** section, import five Schedules from the **OpCon-Dev** Server

### Instructions

#### Import Schedules from the OpCon-Training Environment

1.  In the **Schedules** section, click on the **Import** option
2.  In the **Select OpCon server** dropdown, select the ```OpCon-Dev``` Server
3.  Click the **Next** button 
4.  On the **Select a Schedule to Import** screen, holding the CNTL key down, select the following four Schedules on the left side of the window:
  * Congo Inventory Management 
  * Congo Inventory Reports
  * Congo Payroll Payments
  * HR Import 
5.  Click the **>** button to move the schedule to the right side of the window.
6.  Click the **Next** button
7.  On the **Summary** screen: 
  * Validate that the correct Server is selected in the **OpCon Server** field
  * Select the **Include Sub-Schedules** checkbox
  * Validate that the **five schedules** listed in the **Schedule** section

:::note

Five schedules were imported because **HR Import** contains a sub-schedule, **HR Import Processing**, and we **Included Sub-Schedules** in the** Summary** screen.

:::

8.	Click the **Finish** button
9.	In the **Review Result of Check-In** window, confirm the correct number of Schedules were imported and that the Status of each is listed as **SUCCESS**
10.	Click the **Close** button
11. Stay logged in as **az-win10-deploy\SMAUSER** for the next exercise.

:::info Video Walkthrough

[Import Schedules](../static/imgdeploy/Deploy_ImportSchedules.mp4)

:::