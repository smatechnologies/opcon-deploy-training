---
sidebar_label: 'Deploy Transformations'
hide_title: 'false'
---

## Deploy - Transformations

* Transformations provide the capability to modify the contents of a Schedule or Package Definition during deployment
    * This allows a single Schedule or Package Definitions to be deployed to multiple OpCon Systems

* Transformation Rules are Versioned and stored in the Database
    * Using multiple Transformation Rules is supported

* Transformation Rule names must be unique within the Environment
    * A rule is never overwritten - a new Version is created

* There are three levels of Transformation possible
    * Default Rules associated with an OpCon System
    * Default Rules associated with a Package
    * Transformation Rules selected during the Deployment Phase

### Transformation Storage

* Transformation Rules are defined using JSON format
    * The JSON file contains both required paramaters and optional parameters based on the TagID

![Deployimg047(/imgdeploy/Deployimg047.png)

###### (Click Image to Enlarge)

* ```TagID```
    * Defines what Definition to change
* ```currentValue```
    * Defines what must be changed
* ```newValue```
    * Defines what the New Value should be if there is a match
* ```partialUpdate```
    * Indications whether or not the Update is partial
* ```scheduleName```
    * For some Schedule related ```TagIds```it indicates that this change should only be for the Named Schedule
    * Supports wildcard ```SABC*``` indicating this can be applied to all Schedule beginning with the character sequence ```SABC```
* ```jobName```
    * For some Job related ```TagIds``` it indicates that this change should only be for the named Job
    * Supports wildcard ```JABC*``` indicating that this could be applied to all Jobs beginning with the characer sequence ```JABC```
* ```currentValueContents```
    * Used with Properties, Resources, and Thresholds to define the contents to be changed
* ```newValueContents```
    * Used with Properties, Resources, and Thresholds to define what the Value should be if there is a match


* Special Tags/TagIDs
    * ```environment```
        * Can be used to create a new Version of the Schedule in the same OpCon Environment
        * The Value is prefixed to the Schedule Name, any Global Properties, Thresholds, and Resources to create a unique Instance of the Schedule
    * ```Frequency_Use_Existing_Definitions```
        * Allows a Frequency Definition to be changed
        * Typically used during Migration projects to allow the real Frequency Definition to be entered before Final Testing
    *   ```partialUpdate```
        * Indicates if an Exact Match is required or only a Partial Match is required
        * Care should be taken when using this ```TagID``` as it is possible that you may change items in unintended Definitions
        * ```jobName``` and ```scheduleName``` Tags should be used to limit the scope of the change
    *   ```Windows_User```
        * This Tag is used to change the ```Window User``` of the Job Definition

Supports the following Tags:

* ```jobName```   
    * _Optional_: When present indicates the Job of group of Jobs with which the Rule is associated
    * A group of Jobs is defined by using a wildcard character in the Job Name (Ex. - JOB0100 or JOB01* for all jobs starting with the characters JOB01)

* ```currentValue```
    * _Required_: Contains the name of the ```Windows User``` in the Job Definition

* ```newValue```
    * _Required_: The Value to insert in the Definition if the ```currentValue``` matches the Value in the Definition

* ```partialUpdate```
    * Indicates if the match to be performed is the complete Definition or a partial Definition (Value is ```True``` or ```False```; default is ```False```)