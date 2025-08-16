---
sidebar_label: 'Exercise 3'
---

## Deploy Exercise 3: Deploy Preferences

### Objective

Check and update Deploy preferences

### Summary

Configure Deploy to retain ```5``` version and prevent the updating of **Global Properties**, **Schedule Instance Properties**, **Thresholds**, and **Resources**. You will also **prevent deletion** of schedules from development systems after an **Import** is performed.

### Instructions

#### Configure Settings

1.	Open the Deploy Client using the **Administration User**
  * **User:** ```DeployTeamLead```
  * **PWD:** ```deployadmin```
2.	Under the **Administration** section, click **Settings**
3.	Set the **Number of Versions to Retain** to ```5```

#### Configure Rules

4.	Uncheck the **Update Properties Allowed** checkbox
5.	Uncheck the **Update Variables Allowed** checkbox
6.  Uncheck the **Update Schedule Instance Properties Allowed** checkbox
7.  Uncheck the **Delete Schedule from Development System After Import** checkbox
7.	Click the **Save** button to save changes to the **Global Preferences**

:::info Video Walkthrough

[Global Preferences](../static/imgdeploy/Deploy_GlobalPreferences.mp4)

:::