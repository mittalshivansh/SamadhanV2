# Order listing

{% api-method method="get" host="https://host" path="/api/order/OrderSrList" %}
{% api-method-summary %}
getOrderAndSr
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get free cakes.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="ci" type="number" required=false %}
center id
{% endapi-method-parameter %}

{% api-method-parameter name="ts" type="number" required=false %}
timestamp
{% endapi-method-parameter %}

{% api-method-parameter name="pn" type="number" required=false %}
page no
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}
	
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Sr list.
{% endapi-method-response-example-description %}

```javascript
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
          "serviceLine": 2,
          "serviceTypeId": 1,
          "LMD": 1557337560000
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
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



