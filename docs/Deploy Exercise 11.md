---
sidebar_label: 'Deploy Exercise 11'
hide_title: 'false'
---

## Deploy Exercise 11: Steps to Set Up a Transformation Rule

### Objective:

Use the **Windows Authentication** login to Create Transformation Rules in the Deploy Client

- Create a Rule named ```Dev-to-QA-Machines```
- Within the Rule, create two ```Job: Machine Name``` Transformations
  - Transform the ```OpCon-Dev``` machine to ```OpCon-QA```
  - Transform the ```Susevm1``` machine to ```Susevm```

### Instructions

#### Create a simple Transformation Rule that will allow you to change Machine Names in Jobs from Schedules imported from the OpConTraining Environment to Machines available in the OpCon-Dev Environment when Deploying to the OpCon-Dev Environment

1.	Open the Deploy Client using the **Windows Authentication** login
2.  Click on the **Create/Edit** link in the **Transformation Rules** section
3.	Select the **Add** button to enable the ability to enter information into the various text boxes
4.	Give the Transformation Rule a name by typing ```Dev-to-QA-Machines``` in the **Name** text box
5.	Add a description such as, **Will Convert the Machines Names in the Dev Env to Correct Names for the QA Env**, to the Description text box
6.	To add the list of Transformations, click the green ```+``` button - This will open the **Create or Edit a Transformation** screen
7.	From the **Tag ID** dropdown list select **Job: Machine Name**
8.	In the **Current Value** textbox enter ```OpCon-Dev```
9.	In the **New Value** text box enter ```OpCon-QA```
10.	Click the **Save** button
11.	Now add a second transformation that will transform the Machine Name in Jobs that have a Machine Name of ```Susevm1``` to the Machine Name available in the ```OpCon-QA``` Environment which is ```Susevm```
12.	Once the second Transformation has been created, click the **Save** button on the **View or Edit Transformation Rules** screen to save this new Rule
13.	Click the **Close** button to close out this screen

<video width="320" height="240" controls>
  <source src="imgdeploy/Deploy_CreateTransformationRules.mp4" type="video/mp4"></source>
Your browser does not support the video tag.
</video>