---
description: 'Create order.  Important : no order can be created without a sr and a job.'
---

# Order creation

#### Workflow:

* We will have three layers to get the job into existence. Refer the table below.
* Without a job sr cannot exist and without a sr order cannot exist \(for now\)

Case 1 : when no package 

* packageId will be null in case of single service  
* sr will be created in pending state and job also in pending state
* Job will moved to assigned or tentative-schedule\(current system\) after center or service partner is assigned
* Job will move to schedule after machine, operator and time is confirmed 

Case 2 : When package is selected 

* multiple sr corresponding to each service line stage in package will be created.
* package's discount, Mrp, list price will be copied in each sr as record of transaction.
* then the flow will be same as above

should farm's village should be copied to job as farm can be edited later?



Note : Rate will be derived from center  + geography, so it will be like ServiceLine - center - village - rate. 

**Sr status precedence** : pending &lt; in-progress &lt; completed &lt; cancelled &lt; closed

**Job status precedence** : Pending &lt; Tentative &lt; Tentative- Schedule\(or Assigned\) &lt; Schedule &lt; Closed &lt;                     completed

**Order status precedence :** pending &lt; in-progress &lt; completed &lt; cancelled



<table>
  <thead>
    <tr>
      <th style="text-align:left"><b>Order</b>
      </th>
      <th style="text-align:left"><b>Sr/St</b>
      </th>
      <th style="text-align:left"><b>Job</b>
      </th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td style="text-align:left">
        <ul>
          <li><b>farmerId</b>
          </li>
          <li><b>packageID(nullable)</b>
          </li>
          <li><b>Referred type</b>
          </li>
          <li><b>Referred by</b>
          </li>
          <li><b>date</b>
          </li>
          <li><b>status</b>
          </li>
        </ul>
      </td>
      <td style="text-align:left">
        <ul>
          <li><b>serviceTypeId</b>
          </li>
          <li><b>serviceLine</b>
          </li>
          <li><b>Rate</b>
          </li>
          <li><b>businessDevBy</b>
          </li>
          <li><b>Discount</b>
          </li>
          <li><b>Mrp</b>
          </li>
          <li><b>List price</b>
          </li>
          <li><b>status</b>
          </li>
          <li><b>season</b>
          </li>
        </ul>
      </td>
      <td style="text-align:left">
        <p><b>Creation:</b>
        </p>
        <ul>
          <li><b>farmId</b>
          </li>
          <li><b>estimatedArea</b>
          </li>
          <li><b> UOM ID</b>
          </li>
          <li><b>estimatedBilling unit</b>
          </li>
          <li><b>estimatedAmount</b>
          </li>
          <li><b>Tentative date</b>
          </li>
          <li><b>Time range</b>
          </li>
          <li><b>status</b>
          </li>
        </ul>
        <p><b>Assignment: </b>
        </p>
        <p><b> - centerId </b>
        </p>
        <p><b> - Service Partner</b>
        </p>
        <p>&lt;b&gt;&lt;/b&gt;</p>
        <p><b>Scheduling</b>
        </p>
        <ul>
          <li><b>Machine</b>
          </li>
          <li><b>Operator</b>
          </li>
          <li><b>serviceDate</b>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

{% api-method method="post" host="host" path="/api/order/createOrder" %}
{% api-method-summary %}
create order
{% endapi-method-summary %}

{% api-method-description %}
for request body refer the Below Json. 
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
    "client_ID": "dsdsd2323333ed3",
    "id": 1,
    "sr":[
    {"id":1
    "job":[{"id":1}]
    }]
    "status": true
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

```javascript
Request Body : 
{
  "data": [
    {
      "ID": 174928,
      "LMD": 1557337560000,
      "Referred_by": 3,
      "Referred_type": 3,
      "farmerId": 1,
      "packageId": 2,
      "sr": [
        {
          "Discount": 10,
          "Rate": 500,
          "businessDevBy": 2,
          "job": [
            {
              "Machine": 2,
              "Operator": 2,
              "Service_Partner": "",
              "Tentative_date": "epoch time",
              "Time_range": "",
              "UOM_ID": 2,
              "centerId": 3,
              "estimatedAmount": 323,
              "estimatedArea": 2.22,
              "estimatedBilling_unit": 333,
              "farmId": 1,
              "serviceDate": "epoch time",
              "status": "tentative"
            }
          ],
          "serviceLine": 2,
          "serviceTypeId": 1
        }
      ],
      "status": "tentative"
    }
  ]
}
```

