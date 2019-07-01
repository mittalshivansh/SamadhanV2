# Platform Master data

{% api-method method="get" host="http://192.168.1.111:5000/api" path="/Master/GetPlatformData" %}
{% api-method-summary %}
Get Platform Master data
{% endapi-method-summary %}

{% api-method-description %}
This endpoint allows you to get free cakes.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Platform Master successfully retrieved.
{% endapi-method-response-example-description %}

```javascript
{
    "status": true,
    "message": null,
    "data": {
        "MT": [
            {
                "Mst": [
                    {
                        "Mst": null,
                        "Path": null,
                        "ID": 46,
                        "CD": "mh",
                        "NM": "jh jk jk jk"
                    }
                ],
                "Path": null,
                "ID": 41,
                "CD": "Ank",
                "NM": "Ank"
            },
            {
                "Mst": null,
                "Path": null,
                "ID": 48,
                "CD": "CD",
                "NM": "CD-2"
            },
            {
                "Mst": [
                    {
                        "Mst": null,
                        "Path": null,
                        "ID": 55,
                        "CD": "123",
                        "NM": "Abc"
                    }
                ],
                "Path": null,
                "ID": 53,
                "CD": "ff1",
                "NM": "ff1"
            }
        ],
        "MMM": [
            {
                "MT": [
                    1,
                    4,
                    5,
                    6
                ],
                "ID": 1,
                "CD": null,
                "NM": "Mahindra1"
            },
            {
                "MT": [
                    1,
                    4,
                    5
                ],
                "ID": 2,
                "CD": null,
                "NM": "Maschio"
            }
        ],
        "BNK": [
            {
                "ID": 16,
                "CD": "",
                "NM": "Allahabad Bank"
            },
            {
                "ID": 17,
                "CD": "",
                "NM": "Andhra Bank"
            },
            {
                "ID": 18,
                "CD": "",
                "NM": "Axis Bank"
            },
            {
                "ID": 19,
                "CD": "",
                "NM": "Bank of Bahrain and Kuwait"
            }
        ],
        "KYC": [
            {
                "Upload": true,
                "ID": 1,
                "CD": "UID",
                "NM": "Aadhaar Card"
            },
            {
                "Upload": true,
                "ID": 2,
                "CD": "PAN",
                "NM": "PAN"
            }
        ],
        "consts": {
            "AC": 10,
            "AP": 90
        },
        "PL": [
            {
                "ID": 1,
                "CD": "CP",
                "NM": "Center Partner"
            },
            {
                "ID": 2,
                "CD": "CHC",
                "NM": "Custom Hiring Center (CHC)"
            },
            {
                "ID": 9,
                "CD": "FM",
                "NM": "Farmer"
            },
            {
                "ID": 8,
                "CD": "HH",
                "NM": "House Hold"
            },
            {
                "ID": 4,
                "CD": "HP",
                "NM": "Hub Partner"
            },
            {
                "ID": 7,
                "CD": "IP",
                "NM": "Inception"
            },
            {
                "ID": 3,
                "CD": "SP",
                "NM": "Machine Owner"
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



