# Center Master Data

{% api-method method="get" host="http://192.168.1.111:5000/api/" path="Master/GetCenterMasterData?ci=223" %}
{% api-method-summary %}
Get Center Master Data
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get free cakes.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="ci" type="number" %}
223
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Center Master Data successfully retrieved.
{% endapi-method-response-example-description %}

```javascript
{
    "status": true,
    "message": null,
    "data": {
        "SRC": [
            {
                "PTID": [
                    1,
                    2,
                    9,
                    3
                ],
                "ID": 1,
                "CD": null,
                "NM": "Direct"
            },
            {
                "PTID": [
                    4,
                    7,
                    3
                ],
                "ID": 1,
                "CD": null,
                "NM": "DirectEM3"
            },
            {
                "PTID": [
                    1,
                    8,
                    4,
                    7,
                    3
                ],
                "ID": 2,
                "CD": null,
                "NM": "Indirect"
            },
            {
                "PTID": [
                    8,
                    4,
                    7,
                    3
                ],
                "ID": 3,
                "CD": null,
                "NM": "Call"
            }
        ],
        "REF": [
            {
                "ID": 1,
                "NM": "BA-1 ARANG (CHHATTISGARH)",
                "ISCon": 1,
                "PTID": 4
            },
            {
                "ID": 2,
                "NM": "BA-1 DCM - HARDOI",
                "ISCon": 1,
                "PTID": 4
            },
            {
                "ID": 3,
                "NM": "BA-1 KESHORIA PATAN-8",
                "ISCon": 1,
                "PTID": 4
            },
            {
                "ID": 4,
                "NM": "BA-1 KHATEGAON & UJJAIN-1",
                "ISCon": 1,
                "PTID": 4
            },
            {
                "ID": 5,
                "NM": "BA-1 KOTA",
                "ISCon": 1,
                "PTID": 4
            },
            {
                "ID": 6,
                "NM": "BA-10 SOHAGPUR",
                "ISCon": 1,
                "PTID": 4
            },
            {
                "ID": 7,
                "NM": "BA-11 BAKTARA",
                "ISCon": 1,
                "PTID": 4
            },
            {
                "ID": 8,
                "NM": "BA-2 BAYAN & NASRULLGANJ-2",
                "ISCon": 1,
                "PTID": 4
            },
            {
                "ID": 9,
                "NM": "BA-2 KAITHUN-9",
                "ISCon": 1,
                "PTID": 4
            },
            {
                "ID": 10,
                "NM": "BA-3 HARDA-3",
                "ISCon": 1,
                "PTID": 4
            }
        ]
    },
    "SyncDate": null,
    "PageSize": null,
    "error": ""
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



