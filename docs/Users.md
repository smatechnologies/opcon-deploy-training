---
sidebar_label: 'Administration and Users'
hide_title: 'false'
---

## Deploy Administration

* Administrative Functions are provided to support the definition of Users, OpCon Systems, and Global Settings
* Administrative Functions have four categories:
  * **Users**
  * **Servers**
  * **Audits**
  * **Settings**

![Deployimg004](../static/imgdeploy/Deployimg004.png)

### Administration - Users

* Deploy requires User definitions to manage processes
  * User management is an Administrative Task and can only be accessed by users who have an Administrator Role
* A **Deploy User** is associated with an **OpCon User** when performing tasks that require access to OpCon Systems

### Deploy Roles

* **Administration:** Users has access to Administration rights and all OpCon Systems
* **All:** Users has access to all OpCon Systems
* **Production:** Users only has access to OpCon Systems defined as Production Systems
* **Non-Production:** Users has access to all OpCon Systems _except_ Production Systems
* **Development:** Users only has access to OpCon Systems defined as Development Systems
* **Test:** Users only has access to OpCon Systems defined as Test Systems _(Test, System Test)_

### User Management

![Deployimg005](../static/imgdeploy/Deployimg005.png)

* The User Management Screen allows User Definitions to be created, updated, or removed
* When defining a User:
  * Insert a Unique **User Name**
  * A **Description** for the User
  * Insert a **Password**
  * Select a **Role**
  * Insert the associated OpCon User and Password
    * The **OpCon User** inserted determines the capabilities the User has when logged into the OpCon System
    * The **OpCon User** and **Password** must exist on all systems that the User will access

:::info

Passwords are inserted in Plain Text and then encrypted by the software upon a save.

:::