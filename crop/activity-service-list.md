---
description: Activity and soil list based on Crop
---

# Activity Service List

{% api-method method="get" host="http://samadhanv2api.em3agri.com/api/" path="crop/ActivityServListByCrop" %}
{% api-method-summary %}

{% endapi-method-summary %}

{% api-method-description %}

{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="CropId" type="number" required=true %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}

{% endapi-method-response-example-description %}

```javascript
{
    "status": true,
    "message": null,
    "data": [
        {
            "ID": 1,
            "CD": "CS",
            "NM": "Crop Selection",
            "Serv":[
                {
                "ID": 57,
                "CD": "SR",
                "NM": "Straw Reaper",
                }
            ]
        },
        {
            "ID": 2,
            "CD": "LP",
            "NM": "Land Preparation",
            "Serv":[
                {
                "ID": 254,
                "CD": "test",
                "NM": "input Service test",
                }
            ]
        }
    ],
    "SyncDate": null,
    "PageSize": null,
    "error": ""
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



