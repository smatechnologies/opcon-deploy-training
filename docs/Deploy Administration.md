---
sidebar_label: 'Deploy Administration'
hide_title: 'false'
---

## Deploy Administration

* Administrative Functions are provided to support the definition of Users, OpCon Systems, and Global Settings

* Administrative Fuctions have four categories:
    - **Users**
    - **Servers**
    - **Audits**
    - **Settings**

![Deployimg004](/imgdeploy/Deployimg004.png)

###### (Click Images to Enlarge)

### Administration - Users

* Deploy requires User definitions to manage processes
    - User management is an Administrative Task and can only be accessed by users who have an Administration Role

* A **Deploy User** is associated with an **OpCon User** when performing tasks that require access to OpCon Systems

### OpCon Deploy Roles

* **Administration** 
    - User has access to Administration rights and all OpCon Systems

* **All**
    - User has access to all OpCon Systems

* **Production**
    - User only has access to OpCon Systems defined as Production Systems

* **Non-Production**
    - User has access to all OpCon Systems _except_ Production Systems

* **Development**
    - User only has access to OpCon Systems defined as Development Systems

* **Test**
    - User only has access to OpCon Systems defined as Test Systems _(Test, System Test)_

### User Management

![Deployimg005](/imgdeploy/Deployimg005.png)

* The User Management Screen allows User Definitions to be created, updated, or removed

* When defining a User:
    - Insert a Unique **User Name**
    - A **Description** for the User
    - Insert a **Password** (Passwords are inserted in Plain Text and encrypted by the software)
    - Select a **Role**
    - Insert the associated OpCon User and Password (Passwords are inserted in Plain Text and encrypted by the software)
        - The **OpCon User** inserted determines the capabilities the User has when logged into the OpCon System
        - The **OpCon User** and **Password** must exist on all systems that the User will access