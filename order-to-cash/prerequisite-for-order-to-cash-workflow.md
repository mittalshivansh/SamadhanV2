# Prerequisite for Order to cash workflow

#### Prerequisite Action Points

* [Package listing and api](package-listing.md)
* add service list in [center meta-data api](center-metadata-changes.md)
* add business rules list in [center meta data api](center-metadata-changes.md)
* [Permission Management System](permission-management.md) \(To be discussed\)



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

