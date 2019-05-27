---
description: 'Create or update farmer machine, Kyc update of farmer'
---

# Order creation

{% api-method method="post" host="host" path="/api/order/createOrder" %}
{% api-method-summary %}
create order
{% endapi-method-summary %}

{% api-method-description %}
create farmer macine
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="machine\_type" type="number" required=false %}

{% endapi-method-parameter %}

{% api-method-parameter name="machine\_make" type="string" required=false %}

{% endapi-method-parameter %}

{% api-method-parameter name="model\_year" type="string" required=false %}

{% endapi-method-parameter %}

{% api-method-parameter name="available" type="string" required=false %}
is available for rent
{% endapi-method-parameter %}

{% api-method-parameter name="owned" type="boolean" required=false %}
machine owned or leased
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

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

{% api-method method="get" host="host/" path="api/Farmer/GetFarmerMachine" %}
{% api-method-summary %}
Get Farmer Machine
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
  "status": true,
  "message": "",
  "data": [
   {
      "ID": 0,
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
          "serviceLine": 2,
          "serviceTypeId": 1,
          "LMD": 1557337560000
        }
      ],
      "status": "tentative"
    }
  ],
  "SyncDate": 1557337560000,
  "PageSize": 50,
  "error": ""
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}
