# Crop Activity Service Link

{% api-method method="post" host="http://samadhanv2api.em3agri.com/api/" path="crop/CropActivityServiceList" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="" type="string" required=false %}
{  
    "UID": 1,  
     "CROP": 1,  
     "AcServ":  
\[ {   
         "AC": "1",               "SERV": {1,2,3},  
 },   
{   
     "AC": "2",   
"SERV": {2,3,4},  
} \]   
}
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
    "message": "Crop activity service linked successfully.",
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



