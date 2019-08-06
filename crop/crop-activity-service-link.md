# Crop Activity Service Link

{% api-method method="post" host="http://samadhanv2api.em3agri.com/api/" path="crop/InsertCropActivityService" %}
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
         "AC": "1",               "SERV": \[{  
       ID: 1,  
       IsChecked: true  
       },  
     {   
         ID: 2,  
IsChecked: false}\]  
 },   
{   
     "AC": "2",   
"SERV": \[{   
ID: 2,  
IsChecked: true   
}, {   
ID:3,   
IsChecked: false}\]  
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



