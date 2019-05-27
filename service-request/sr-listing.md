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
{% api-method-path-parameters %}
{% api-method-parameter name="id" type="string" %}
ID of the cake to get, for free of course.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-headers %}
{% api-method-parameter name="Authentication" type="string" required=true %}
Authentication token to track down who is emptying our stocks.
{% endapi-method-parameter %}
{% endapi-method-headers %}

{% api-method-query-parameters %}
{% api-method-parameter name="recipe" type="string" %}
The API will do its best to find a cake matching the provided recipe.
{% endapi-method-parameter %}

{% api-method-parameter name="gluten" type="boolean" %}
Whether the cake should be gluten-free or not.
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



