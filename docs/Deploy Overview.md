---
sidebar_label: 'Deploy Overview'
hide_title: 'false'
---

## Deploy Overview


* Opcon Deploy is a Change Management compliance application that deploys Schedule definitions between OpCon environments in a controlled and consistent manner

* Utilizes a central repository that contains:
    - Schedule Definitions
    - Transformation Rules
    - Additional required configuration information

* The Deploy Database/Repository implements:
    - Versioning of Schedules, Scripts, and Transformation Rules
    - The concept of a **Package** that can be used to group Schedules to ensure consistent deployment
    - Auditing on all User actions
    - Transformation capabilities allowing a single Definition to be deployed to multiple systems with automatic target system adjustments

* Updates are performed within a single transaction 
    - Allows the existing Definition to be in a consistent state should error occur
    - Provides simulated deployment which performs an error check and reports any issues
    - Provides rollback capabilities to quickly restore a deployment to a previous stable version
    - Provides **Batch Deployment** capability allowing deployments to be scheduled for future dates and times

![Deployimg002](/imgdeploy/Deployimg002.png)

###### (Click Images to Enlarge)


### Server Communication

* Uses a new RESTful web server (ImpEx2 Server) that provides communication between Deploy and OpCon systems
* Provides User, Server, and Global settings
* **Users** are associated with **_Roles_** which determine the functions available to the selected User 
    - Deploy Users are mapped to OpCon system Users
* Servers are associated with **Types** which determine the Users with access to the Server via User Roles
    - Servers are mapped to specified OpCon systems

![Deployimg003](/imgdeploy/Deployimg003.png)

