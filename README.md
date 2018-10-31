# Initial page

{% api-method method="get" host="https://api.aedifion.io" path="/v2/meta/endpoints" %}
{% api-method-summary %}
Get a list of available endpoints
{% endapi-method-summary %}

{% api-method-description %}
Returns a list of available IDs and their names
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
List of all available endpoints are returned
{% endapi-method-response-example-description %}

```javascript
[
  {
    "id": 0,
    "path": "string",
    "request_method": "string",
    "summary": "string"
  }
]
```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorised Access
{% endapi-method-response-example-description %}

```javascript
{
  "error": "string",
  "operation": "",
  "success": false
}
```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}



