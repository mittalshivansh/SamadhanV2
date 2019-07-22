# Soil List

{% api-method method="get" host="http://samadhanv2api.em3agri.com/api/" path="soil/SoilList" %}
{% api-method-summary %}
Get Soil List
{% endapi-method-summary %}

{% api-method-description %}
Soil List
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
    "status": true,
    "message": null,
    "data": [
        {
            "ID": 1,
            "CD": null,
            "NM": "sandy_loam"
        },
        {
            "ID": 2,
            "CD": null,
            "NM": "loam"
        },
        {
            "ID": 3,
            "CD": null,
            "NM": "alluvial"
        },
        {
            "ID": 4,
            "CD": null,
            "NM": "red"
        },
        {
            "ID": 5,
            "CD": null,
            "NM": "laterite"
        },
        {
            "ID": 6,
            "CD": null,
            "NM": "desert"
        },
        {
            "ID": 7,
            "CD": null,
            "NM": "black"
        }
    ],
    "SyncDate": null,
    "PageSize": null,
    "error": ""
}
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
Could not find soil
{% endapi-method-response-example-description %}

```javascript
{
    "status": false,
    "message": "No Record Found. Please try again.",
    "data": null
    "SyncDate": null,
    "PageSize": null,
    "error": ""
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



