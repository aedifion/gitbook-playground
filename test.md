# Test

{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/{project\_id}/alert" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/alert   
{% endapi-method-summary %}

{% api-method-description %}
  
Creates a new alert with the specified details. The following parameters can/must be provided:**Note:** When using the example JSON from this documentation, the json string needs to be reduced to the alert inputs needed, i.e. the line "JSON Example for \[...\]" nees to be erased. Please check consistence of brackets so that the outgoing json is well defined.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The numeric id of the project on which to create the alert.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter name="newalert" type="object" required=true %}
  
The details of the alert to create as documented in the description above.
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The newly created alert is returned in the 'resource' field and 'operation' will indicate a 'create' operation.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unsuccessful request. The error is returned in the 'error' field and 'operation' will indicate a 'create' operation.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=415 %}
{% api-method-response-example-description %}
  
Unsuccessful request. The error is returned in the 'error' field and 'operation' will indicate a 'create' operation.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

