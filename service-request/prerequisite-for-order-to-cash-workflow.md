# Prerequisite for Order to cash workflow



**Package :**

* Name
* validity
* structure/ b.line/ BA
* MRP/discount/List price

**package/bundle**

* serviceId
* Stage
* packageId
* MRP/discount/List price

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

