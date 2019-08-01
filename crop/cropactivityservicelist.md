# CropActivityServiceList

{% api-method method="get" host="http://samadhanv2api.em3agri.com/api/" path="crop/CropActivityServiceList?CropID=1" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="CropId" type="string" required=true %}

{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
 [{
   "AC": "1",               
   "SERV": [1,2,3],
 }, 
{
   "AC": "2",               
   "SERV": [2,3,4],
 }] 
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



