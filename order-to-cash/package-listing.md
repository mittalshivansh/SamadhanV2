# Package Listing

#### Workflow:

* We can link multiple center with a package, center id will be passed to fetch package list.
* package can only be linked if all services under package are available at that center, vice-versa package will be deactivated on a centre if after sometime service is deactivated.



{% api-method method="get" host="https://host" path="/api/order/packageList" %}
{% api-method-summary %}
get package list
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get packages list.
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
      "Name": "",
      "price": 3,
      "discount": 3,
      "validity": 1,
      "services": [
        {
          "serviceId": 10,
          "Stage": 500,
          "price": 3,
          "discount": 3
        }
      ]
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

