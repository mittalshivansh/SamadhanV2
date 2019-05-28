# Prerequisite for Order to cash workflow

#### Action Points

* package listing api
* add service list in center meta-data api
* add business rules list in center meta data api



**Reference for Schema level at backend  :**

**Service Type**

* typeName
* typeId

**ServiceLine**

* name
* serviceTypeId
* Code
* rateType
* standardConversion from acres
* standardTimeConsumption

**Service - BusinessLine \(need to be normalized \)**

* serviceId
* BA
* Crop
* Soil
* machineType

**BusinessLine-Rules**

* Center min advance
* Advance stage : sr creation or job scheduling
*  Sr creation aprroval required?
*  Job schedule service partner approval required ?

