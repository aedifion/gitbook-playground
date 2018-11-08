# Test

<br/>{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/{project_id}/alert" %}
<br/>{% api-method-summary %}<br/>
/v2/project/{project_id}/alert
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Creates a new alert with the specified details. The following parameters can/must be provided:
  - **name**, the name of the alert. The name needs to be unique within a project. In case it is not, the error message will inform about it. [mandatory]
  - **telegram_chatid**, id of a Telegram chat which alerts are sent to [optional]
  - **email**, single email address or comma separated list of email addresses which alerts are sent to [optional]
  - **alert_type**, 'throughput' or 'threshold' [mandatory]. Alerts of type 'throughput' will notify when the total number of received observations per datapoint or per whole project undercut a lower limit per specified time interval. Alerts of type 'threshold' will notify when the measured values exceed or undercut a specified threshold.
  - Special parameters for 'alert_type' = 'throughput':
    - **dataPointID**, alphanumeric id of datapoint on which to measure throughput. If not provided, throughput of the whole project is measured. [optional]
    - **threshold_info**, first threshold for which the alarm is fired, e.g., when throughput is slightly lower than usual. [mandatory]
    - **thredholw_warn**, second thresholdfor which the alarm is fired, e.g., when throughput is significantly lower than usual. [mandatory]
    - **threshold_crit**, third threshold for which the alarm is fired, e.g., when throughput is critically low. [mandatory]
    - **period**, time period over which to measure throughput (examples: "1h", "30s", "10m") [mandatory]
  - Special parameteres for 'alert_type' = 'threshold':
    - **dataPointID**, alphanumeric id of datapoint on which to set thresholds [mandatory]
    - **threshold_dead**, the threshold below which sensor is considered DEAD [mandatory]
    - **threshold_ok**, the threshold below which measured values are considerd OK and the alert is reset [mandatory]
    - **threshold_crit**, the threshold above which measured values are considered CRITICAL and the alert fires [mandatory]
    - **threshold_order**, order of the thresholds. 'asc' as described above, or 'desc' to reverse order of DEAD, OK, and CRITICAL levels (basically, flips all comparisons from < to >= and <= to >) [optional, default='asc']
    - **period**, the time period after which an alert is resent when in state CRITICAL state (examples: "1h", "30s", "10m") [mandatory]

**Note:** When using the example JSON from this documentation, the json string needs to be reduced to the alert inputs needed, i.e. the line "JSON Example for [...]" nees to be erased. Please check consistence of brackets so that the outgoing json is well defined.

<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The numeric id of the project on which to create the alert.{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="newalert" type="object" required=true%}
<br/>The details of the alert to create as documented in the description above.{% endapi-method-parameter %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The newly created alert is returned in the 'resource' field and 'operation' will indicate a 'create' operation.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unsuccessful request. The error is returned in the 'error' field and 'operation' will indicate a 'create' operation.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=415 %}
<br/>{% api-method-response-example-description %}
<br/>Unsuccessful request. The error is returned in the 'error' field and 'operation' will indicate a 'create' operation.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>
