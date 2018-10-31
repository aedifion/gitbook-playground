# Initial page
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/meta/endpoints" %}
<br/>{% api-method-summary %}<br/>
Get a list of available endpoints.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns a list of available endpoint IDs and their names.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. A list of all available endpoint IDs and their names is returned.
{% endapi-method-response-example-description %}
```


<br/>{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to get.
{% endapi-method-response-example-description %}
```


<br/>{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
