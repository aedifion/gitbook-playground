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
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to get.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/company" %}
<br/>{% api-method-summary %}<br/>
Get all projects and users defined in the company.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns a list of projects and users defined for the queried company.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. Returns a list of roles in the queried project.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/company/roles" %}
<br/>{% api-method-summary %}<br/>
Get all roles defined in the company.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns a list of roles defined for the queried company.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. Returns a list of roles in the queried company.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="post" host="https://api.aedifion.io" path="/v2/company/role" %}
<br/>{% api-method-summary %}<br/>
Create a new role for the logged user's company.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Creates a new role for the company, user is logged in with.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="role_definition" type="None" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. Returns details of created role.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'post'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
