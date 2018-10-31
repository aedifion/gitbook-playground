# Initial page
{% api-method method="get" host="https://api.aedifion.io" path="/v2/meta/endpoints" %}
{% api-method-summary %}
Get a list of available endpoints.
{% endapi-method-summary %}
{% api-method-description %}
Returns a list of available endpoint IDs and their names.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. A list of all available endpoint IDs and their names is returned.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to get.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
