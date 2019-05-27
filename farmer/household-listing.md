# HouseHold Listing

{% api-method method="get" host="https://host" path="/api/Farmer/HouseHoldList" %}
{% api-method-summary %}
Get HouseHold
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get all households with farmers and farms
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
household successfully retrieved.
{% endapi-method-response-example-description %}

```javascript
{
    "status": true,
    "message": "",
    "data": [
        {
            "ID": 174928,
            "Nm": "ankit khurana",
            "Farmer": [
                {
                    "Vill": "Sarsawa",
                    "HHN": "ankit khurana",
                    "phto": null,
                    "ID": 174929,
                    "Nm": "ankit khurana",
                    "Fn": "Mahendra khurana",
                    "Mo": "9871954626",
                    "Gi": 4414,
                    "HH": 174928,
                    "MOV": false
                }
            ],
            "Farm": [
                {
                    "ID": 41,
                    "Nm": "Pedal la pade",
                    "Lm": "near pani ki tanki",
                    "Sz": 3,
                    "UOM": "Acre",
                    "Gi": 4414,
                    "Vill": "Sarsawa",
                    "Ac": true,
                    "Si": 4,
                    "Soil": "Sarsawa",
                    "Khn": null
                }
            ],
            "LMD": 1557337560000
        }
    ],
    "SyncDate": 1557337560000,
    "PageSize": 50,
    "error": ""
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



