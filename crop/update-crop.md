# Update Crop

{% api-method method="post" host="http://samadhanv2api.em3agri.com/api/" path="soil/UpdateSoil" %}
{% api-method-summary %}
Update Crop
{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="" type="string" required=false %}
  
      "ID":10,  
      "Cd":"t1",  
      "Nm":"Test 2",  
      "Type":"K",  
        "Uid":1,  
        "Soil":\[2,3,4\]  
 }  
  
K-Kharif, R-Rabi, Z-Zaid
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
    "status": true,
    "message": "Crop Updated successfully.",
    "data": null,
    "SyncDate": null,
    "PageSize": null,
    "error": ""
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



