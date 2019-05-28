---
description: 'Create or update farmer machine, Kyc update of farmer'
---

# Order creation

```text
{
  "PageSize": 50,
  "SyncDate": 1557337560000,
  "data": [
    {
      "ID": 174928,
      "LMD": 1557337560000,
      "Referred_by": 3,
      "Referred_type": 3,
      "farmerId": 1,
      "packageId": 2,
      "sr": [
        {
          "Discount": 10,
          "Rate": 500,
          "businessDevBy": 2,
          "job": [
            {
              "Machine": 2,
              "Operator": 2,
              "Service_Partner": "",
              "Tentative_date": "epoch time",
              "Time_range": "",
              "UOM_ID": 2,
              "centerId": 3,
              "estimatedAmount": 323,
              "estimatedArea": 2.22,
              "estimatedBilling_unit": 333,
              "farmId": 1,
              "serviceDate": "epoch time",
              "status": "tentative"
            }
          ],
          "serviceLine": 2,
          "serviceTypeId": 1
        }
      ],
      "status": "tentative"
    }
  ],
  "error": "",
  "message": "",
  "status": true
}
```

{% api-method method="post" host="host" path="/api/order/createOrder" %}
{% api-method-summary %}
create order
{% endapi-method-summary %}

{% api-method-description %}
for request body refer the above Json. 
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Cake successfully retrieved.
{% endapi-method-response-example-description %}

```javascript
{
    "client_ID": "dsdsd2323333ed3",
    "id": 1,
    "status": true
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find a cake matching this query.
{% endapi-method-response-example-description %}

```javascript
{
    "message": "Ain't no cake like that."
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

