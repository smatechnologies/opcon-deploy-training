---
sidebar_label: 'Deploy Deployment Simulation'
hide_title: 'false'
---

## Deployment - Simulation

<a href="imgdeploy/Deployimg066.png" target="_blank"><img src="imgdeploy/Deployimg066.png" width="600"></img></a>

###### (Click Images to Enlarge)

* The **Simulation** feature performs a Test Deployment
    * Checks for Schedule Definition matching
    * Checks for SubSchedules
    * Checks for Machines
        * Primary, alternates, file transfer, (source & destination)
    * Checks for Machine Groups
    * Checks for Batch Users with IBMi, MCP, OpenVMS, SQL, Windows, and UNIX Jobs
    * Checks for missing External Dependencies
    * Checks through Job Types for Agent features:


```Unix```

* Embedded Scripts

* File Watcher

* Job Output Parsing

* Environmental Variables

```Windows```

* Embedded Scripts

* File Watcher
 
* Job Output Parsing
 
* Environmental Variables

* Shell Execution

```IBMi```

* File Arrival Job



* Returns a Report on the Simulation Check containing:
    * Schedule Comparisom
    * SubSchedule Check
    * Machine Check
    * Machine Group Check
    * Batch User Check
    * Job Machine Feature Requirements Check
    * Dependent Job Check

<a href="imgdeploy/Deployimg067.png" target="_blank"><img src="imgdeploy/Deployimg067.png" width="500"></img></a>    

* If an error is encountered, the font color of the Report Header will be **Red**
    * If Definitions mismatch, the differences will be displayed
    * If there are missing items, they will be displayed within the expected session

<a href="imgdeploy/Deployimg068.png" target="_blank"><img src="imgdeploy/Deployimg068.png" width="500"></img></a>