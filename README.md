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
<br/>{% api-method method="put" host="https://api.aedifion.io" path="/v2/company/role/{role_id}" %}
<br/>{% api-method-summary %}<br/>
Updates an existing role for the company.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Updates an existing role for the company.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="role_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
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
<br/>Successful operation. Returns details of edited role.
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
<br/>{% api-method method="delete" host="https://api.aedifion.io" path="/v2/company/role/{role_id}" %}
<br/>{% api-method-summary %}<br/>
Delete an existing role for the company.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Deletes an existing role for this company.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="role_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The deleted project is returned within the 'resource' field and 'operation' will indicate a 'delete' operation
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
<br/>{% api-method method="post" host="https://api.aedifion.io" path="/v2/company/role/{role_id}/user/{user_id}" %}
<br/>{% api-method-summary %}<br/>
Assign a role to a user.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Assigns role with its id 'role_id' to user with her/his id 'id'.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="user_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="role_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The newly created relation between 'user' and 'role' is returned in the 'resource' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="delete" host="https://api.aedifion.io" path="/v2/company/role/{role_id}/user/{user_id}" %}
<br/>{% api-method-summary %}<br/>
Removes a role from a user.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Removes role with id 'role_id' from user with id 'id'.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="user_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="role_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The deleted relation between 'user' and 'role' is returned in the 'resource' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/token" %}
<br/>{% api-method-summary %}<br/>
Get authentication token.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns an authentication token which contains the encrypted user name and password. The token can be used instead of HTTP basic auth by using the token as user name and leaving the password field empty.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="validity" type="number" required=False%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="scope" type="string" required=False%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Success
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="post" host="https://api.aedifion.io" path="/v2/user" %}
<br/>{% api-method-summary %}<br/>
Create a new user.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Creates a new user with the specified details.
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
<br/>{% api-method-parameter name="user" type="None" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The newly created user is returned in the 'resource' field and the 'operation' will indicate a CREATE operation.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unsuccessful request. The error is returned in the 'error' field.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/user" %}
<br/>{% api-method-summary %}<br/>
Get logged in user's details.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns the details of the logged in user.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Success
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="put" host="https://api.aedifion.io" path="/v2/user" %}
<br/>{% api-method-summary %}<br/>
Update the details of the logged in user.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Updates the details of the specified user (specification by authentication credentials).
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
<br/>{% api-method-parameter name="user" type="None" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Success
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="delete" host="https://api.aedifion.io" path="/v2/user" %}
<br/>{% api-method-summary %}<br/>
CAUTION: Deletes logged in user.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Deletes the logged in user and all his/her resources - DANGER to suspend important accounts!
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The deleted user is returned within the 'resource' field and 'operation' will indicate a DELETE operation.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized access.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/user/resetPassword" %}
<br/>{% api-method-summary %}<br/>
Resets user's password.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Triggers a confirmation mail to the given email address that allows to reset user's password. Please also check for the email in your junk mail folder.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="email" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=404 %}
<br/>{% api-method-response-example-description %}
<br/>User not found.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=500 %}
<br/>{% api-method-response-example-description %}
<br/>Out of service.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/user/projects" %}
<br/>{% api-method-summary %}<br/>
Get user's projects.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns a list of all projects that the user is authorized for.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. A list of projects that the user is authorized to access is returned.
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
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/user/favorites" %}
<br/>{% api-method-summary %}<br/>
Get user's favorite data points.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns a list of data points that the user marked as his/her favorites.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. A list of all data points that the current user marked as favorites is returned.
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
<br/>{% api-method method="post" host="https://api.aedifion.io" path="/v2/user/plotview" %}
<br/>{% api-method-summary %}<br/>
Add a plotview.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Creates a new plotview and adds it to the list of plotviews for this user.
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
<br/>{% api-method-parameter name="plotview" type="None" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The user and newly created plotview are returned in the 'resource' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/user/plotviews" %}
<br/>{% api-method-summary %}<br/>
Get user's plotviews.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns a list of all plotviews that the user has specified or shared.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. A list of all plotViews for the current user is returned.
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
<br/>{% api-method method="put" host="https://api.aedifion.io" path="/v2/user/plotview/{plotview_id}" %}
<br/>{% api-method-summary %}<br/>
Update a plotview.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Updates a plotview for this user.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="plotview_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="plotview" type="None" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The updated plotView is returned in the 'resource' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="delete" host="https://api.aedifion.io" path="/v2/user/plotview/{plotview_id}" %}
<br/>{% api-method-summary %}<br/>
Delete a plotview.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Deletes a plotview for this user.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="plotview_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The newly created plotView is returned in the 'resource' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="post" host="https://api.aedifion.io" path="/v2/project" %}
<br/>{% api-method-summary %}<br/>
Create a new project.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Creates a new project with the specified details.
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
<br/>{% api-method-parameter name="project" type="None" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The newly created project is returned in the 'resource' field and the 'operation' will indicate a CREATE operation.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unsuccessful request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}" %}
<br/>{% api-method-summary %}<br/>
Get project's details.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns the details of the queried project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. Returns the project, the company that owns this project, and a list of data point keys associated with this project.
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
<br/>{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project_id}" %}
<br/>{% api-method-summary %}<br/>
Update project's details.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Updates the details of the specified project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="project" type="None" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The updated project is returned within the 'resource' field and 'operation' will indicate a 'update' operation.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/{project_id}" %}
<br/>{% api-method-summary %}<br/>
Delete project.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Deletes the specified project and all its associated resources.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The deleted project is returned within the 'resource' field and 'operation' will indicate a 'delete' operation.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}/roles" %}
<br/>{% api-method-summary %}<br/>
Get all roles defined in the project.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns a list of roles defined for the queried project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
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
<br/>{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/{project_id}/role" %}
<br/>{% api-method-summary %}<br/>
Create a new role for this project.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Creates a new role for this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
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
<br/>{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project_id}/role/{role_id}" %}
<br/>{% api-method-summary %}<br/>
Updates an existing role for this project.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Updates an existing role for this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="role_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
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
<br/>Successful operation. Returns details of edited role.
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
<br/>{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/{project_id}/role/{role_id}" %}
<br/>{% api-method-summary %}<br/>
Delete an existing role for this project.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Deletes an existing role for this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="role_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The deleted project is returned within the 'resource' field and 'operation' will indicate a 'delete' operation
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
<br/>{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/role/{role_id}/user/{user_id}" %}
<br/>{% api-method-summary %}<br/>
Assign a role to a user.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Assigns role with its id 'role_id' to user with her/his id 'id'.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="user_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="role_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The newly created relation between 'user' and 'role' is returned in the 'resource' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/role/{role_id}/user/{user_id}" %}
<br/>{% api-method-summary %}<br/>
Removes a role from a user.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Removes role with id 'role_id' from user with id 'id'.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="user_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="role_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The deleted relation between 'user' and 'role' is returned in the 'resource' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/{project_id}/datapointkey" %}
<br/>{% api-method-summary %}<br/>
Create new data point key in project.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Creates a new data point key in this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="datapointkey" type="None" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The newly created data point key is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}/datapointkeys" %}
<br/>{% api-method-summary %}<br/>
Get list of data point keys associated with project.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns a list of all data point keys that have been created in this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Success
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
<br/>{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project_id}/datapointkey/{datapointkey_id}" %}
<br/>{% api-method-summary %}<br/>
Updates a data point key.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Updates the specified data point key associated with the project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="datapointkey_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="datapointkey" type="None" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The updated data point key is returned within the 'resource' field and 'operation' will indicate a 'update' operation.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/{project_id}/datapointkey/{datapointkey_id}" %}
<br/>{% api-method-summary %}<br/>
Deletes a data point key associated with the project.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Deletes the specified data point key from the list of data point keys available in this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="datapointkey_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Success
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}/datapoints" %}
<br/>{% api-method-summary %}<br/>
Get list of data points in this project.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns a list of all data points that have been created in this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Success
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unsuccessful operation. Details on the error are returned in the 'error' field.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}/datapoints/favorites" %}
<br/>{% api-method-summary %}<br/>
Get list of favorited data points in this project.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns a list of all favorite data points that have been created in this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Success
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unsuccessful operation. Details on the error are returned in the 'error' field.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}/datapoints/renamings" %}
<br/>{% api-method-summary %}<br/>
Get list of data points and their renamings in this project.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns a list of all data points and their renamings that have been created in this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="datapointkey_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Success
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unsuccessful operation. Details on the error are returned in the 'error' field.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/{project_id}/tag" %}
<br/>{% api-method-summary %}<br/>
Create a new tag.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Creates a new tag that can then be assigned to data points in this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="tag" type="None" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The newly created tag is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}/tags" %}
<br/>{% api-method-summary %}<br/>
Get all data point tags in this project.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns a list of all data point tags that have been created in this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. A list of all tags for data points in the specified project is returned.
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
<br/>{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project_id}/tag/{tag_id}" %}
<br/>{% api-method-summary %}<br/>
Update an existing tag.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Updates an existing tag associated with this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="tag_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="tag" type="None" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The updated tag is returned in the 'resource' field and the 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/{project_id}/tag/{tag_id}" %}
<br/>{% api-method-summary %}<br/>
Delete a tag.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Deletes an existing tag associated with this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="tag_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The deleted tag is returned in the 'resource' field and the 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}/datapoints/byTag" %}
<br/>{% api-method-summary %}<br/>
Get all data points in this project with a given tag.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns a list of all data points by tag that have been initialized in this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="key" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="value" type="string" required=False%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="source" type="string" required=False%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="confirmed" type="string" required=False%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. A list of all data points with the given tag in the specified project is returned.
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
<br/>{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/{project_id}/alert" %}
<br/>{% api-method-summary %}<br/>
Create a new alert.
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
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="newalert" type="None" required=True%}
<br/>{% endapi-method-parameter %}
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
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}/alerts" %}
<br/>{% api-method-summary %}<br/>
Get all alerts in a project.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns the details of all alerts in a project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. A list of all alerts for the specified project is returned.
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
<br/>{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project_id}/alert/{alert_id}" %}
<br/>{% api-method-summary %}<br/>
Edit an Alert.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Modify alert settings. For more information on parameters and alarms which can be modified, view the endpoint `/v2/project/{id}/alert` (post).
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="alert_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="param" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="value" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The edited alert is returned in the 'resource' field and the 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/{project_id}/alert/{alert_id}" %}
<br/>{% api-method-summary %}<br/>
Delete an alert.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Delete an alert by its ID.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="alert_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The details of the deleted alarm are returned in the 'resource' field and 'operation' will indicate a 'delete' operation.

{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unsuccessful request.
Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'."

{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project_id}/alert/{alert_id}/toggle" %}
<br/>{% api-method-summary %}<br/>
Enable or disable an alert.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Enable or disable an alert.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="alert_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The toggled alert is returned in the 'resource' field and the 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/{project_id}/importTimeseries" %}
<br/>{% api-method-summary %}<br/>
Imports timeseries data from a file
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Imports timeseries data defined in a file.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="format" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="on_error" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The uploaded timeseries is returned in the 'resource' field and the 'operation' will indicate a CREATE operation.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unsuccessful request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/{project_id}/component/" %}
<br/>{% api-method-summary %}<br/>
Add a new component.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Adds a new component to the specified project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="component_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="component_details" type="None" required=False%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The newly added component is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}/component/{componentinproject_id}" %}
<br/>{% api-method-summary %}<br/>
Get a component for the specified project.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Gets a component defined in project along with its pin details.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="componentinproject_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. All component details along with its pin details is returned in the 'resource' field and the 'operation' is set to 'get'.
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
<br/>{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project_id}/component/{componentinproject_id}" %}
<br/>{% api-method-summary %}<br/>
Edit a component in the specified project.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Edits a component for this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="componentinproject_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="component_details" type="None" required=False%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The edited component is returned in the 'resource' field and the 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/{project_id}/component/{componentinproject_id}" %}
<br/>{% api-method-summary %}<br/>
Delete a component in the specified project.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Deletes a component defined in the specified project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="componentinproject_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The details of the deleted component are returned in the 'resource' field and 'operation' will indicate a 'delete' operation.

{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}/components" %}
<br/>{% api-method-summary %}<br/>
Get all components in a project.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Get all components that have been added to the project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. A list of component ids along with their english and german names are returned in the 'resource' field and the 'operation' is set to 'get'.
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
<br/>{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/{project_id}/component/pin/datapoint" %}
<br/>{% api-method-summary %}<br/>
Connects a datapoint to a component's pin.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Connects a datapoint to a component's pin within the specified project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="componentinproject_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="pin_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="dataPointID" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The component with added datapoint is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project_id}/component/pin/datapoint" %}
<br/>{% api-method-summary %}<br/>
Edits a datapoint on a component pin in the specified project.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Edit a datapoint on component pin for the specified project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="componentinproject_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="pin_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="dataPointID" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The component with edited datapoint is returned in the 'resource' field and the 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/{project_id}/component/pin/datapoint" %}
<br/>{% api-method-summary %}<br/>
Delete a datapoint on component pin for the project.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Deletes a datapoint on component pin defined in project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="componentinproject_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="pin_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The details of the deleted datapoint on component are returned in the 'resource' field and 'operation' will indicate a 'delete' operation.

{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/datapoint" %}
<br/>{% api-method-summary %}<br/>
Get details about data point.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Gets the data point including meta information, i.e., whether it is a user's favorite, its renamings and tags.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="dataPointID" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The data point including meta information is returned.
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
<br/>{% api-method method="put" host="https://api.aedifion.io" path="/v2/datapoint" %}
<br/>{% api-method-summary %}<br/>
Change datapoint details.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Modifies datapoint details such as safety bounds for setpoints.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="dataPointID" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="datapoint_details" type="None" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The modified datapoint is returned in the 'resource' field and the 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/datapoint/timeseries" %}
<br/>{% api-method-summary %}<br/>
Get the time series data of a data point.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns the measured time series data for the specified data point
referenced by its name/dataPointID for the time interval specified by **start**
and **end**.
Returns the last (or respectively next) **max** observations, if either **start** nor **end** are provided.

<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="dataPointID" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="start" type="string" required=False%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="end" type="string" required=False%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="max" type="integer" required=False%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="samplerate" type="string" required=None%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. A list of observations for the specified data point is returned.
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
<br/>{% api-method method="post" host="https://api.aedifion.io" path="/v2/datapoint/favorite" %}
<br/>{% api-method-summary %}<br/>
Set a data point as personal favorite.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Sets a data point referenced by its name/dataPointID as a favorite for the user.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="dataPointID" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The newly created favorite is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unsuccessful operation. Details on the error are returned in the 'error' field.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="delete" host="https://api.aedifion.io" path="/v2/datapoint/favorite" %}
<br/>{% api-method-summary %}<br/>
Remove a personal favorite data point.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Removes a data point from the personal favorites of the user.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="dataPointID" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The deleted favorite data point is returned in the 'resource' field and the 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="post" host="https://api.aedifion.io" path="/v2/datapoint/renaming" %}
<br/>{% api-method-summary %}<br/>
Add an alternative name associated with a specific data point key for a data point.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Assigns an alternative name to a data point referenced by its name/dataPointID under the specified data point key id.
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
<br/>{% api-method-parameter name="renaming" type="None" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The newly created renaming is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="put" host="https://api.aedifion.io" path="/v2/datapoint/renaming/{renaming_id}" %}
<br/>{% api-method-summary %}<br/>
Change a renaming.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Changes the alternative name of a data point under a data point key.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="renaming_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="renaming" type="None" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The newly created renaming is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="delete" host="https://api.aedifion.io" path="/v2/datapoint/renaming/{renaming_id}" %}
<br/>{% api-method-summary %}<br/>
Delete an alternative name for a given data point under a given data point key.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Deletes the alternative name for the data point referenced by its name/dataPointID under the specified dataPointKey.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="renaming_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The newly created renaming is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="post" host="https://api.aedifion.io" path="/v2/datapoint/tag" %}
<br/>{% api-method-summary %}<br/>
Add a tag.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Adds a tag to the specified data point.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="dataPointID" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="tag_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The newly created relation (data point, tag) is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="put" host="https://api.aedifion.io" path="/v2/datapoint/tag/{tag_id}" %}
<br/>{% api-method-summary %}<br/>
Update tag associated with data point.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Updates the tag identified by 'id' associated with the data point identified by 'dataPointID' and 'project_id'.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="tag_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="dataPointID" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="tag" type="None" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation.
The updated tag is returned in the 'resource' field and the 'operation' is set to 'update'.

{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unsuccessful request.
Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'."

{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="delete" host="https://api.aedifion.io" path="/v2/datapoint/tag/{tag_id}" %}
<br/>{% api-method-summary %}<br/>
Remove tag from data point.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Removes the tag identified by 'id' from the data point identified by 'dataPointID' and 'project_id'.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="tag_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="dataPointID" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation.
The deleted relation (data point, tag) is returned in the 'resource' field and the 'operation' is set to 'delete'.

{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unsuccessful request.
Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'."

{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="post" host="https://api.aedifion.io" path="/v2/datapoint/setpoint" %}
<br/>{% api-method-summary %}<br/>
Write a setpoint.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Attempts to write 'value' with given 'priority' to the the data point identified by 'dataPointID' and 'project_id'.

This endpoint implements a no-frills, non-acked, stateless, best-effort write service intended for single one-shot setpoint write operations. If you need to write schedules (multiple consecutive setpoints), require acknowledgements, or feedback on the current state of the target datapoint, please refer to `POST/GET/PUT/DELETE /v2/datapoint/schedule`.

**Please note:**
  - Setpoint writing is currently only supported for BACnet.**
  - This endpoint returns '200 - success' if the setpoint operation is authorized and correctly specified. It does not provide any feedback whether the setpoint has actually been written successfully by the remote building network.

<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="dataPointID" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="value" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="priority" type="integer" required=None%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. The setpoint operation has been triggerd but may still fail on the remote side, i.e., the building network.

{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unsuccessful request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'."

{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="post" host="https://api.aedifion.io" path="/v2/datapoint/schedule" %}
<br/>{% api-method-summary %}<br/>
Write a schedule of setpoints for given datapoint.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/> Attempts to write a schedule consisting of different setpoints to the the data point identified by 'dataPointID' and 'project_id'. Returns a unique `reference` for that schedule.
**Note regarding asynchronous communication:**
Since the successful writing of a setpoints in a schedule may require several attempts on the local building network, this api call is asynchronous, i.e., this api call returns *before* the process of writing setpoints in a schedule (and acknowledging it) has been fully concluded. Thus, this api call immediately returns a unique reference that can be used by the caller to query status of this schedule using endpoint `/v2/datapoint/schedule/{id}`.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="dataPointID" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% api-method-parameter name="project_id" type="integer" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="schedule" type="None" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation.
The details of the schedule created according to this operation is returned in the 'resource' field and the 'operation' is set to 'create'.

{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unsuccessful request.
Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'."

{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/datapoint/schedule/{reference}" %}
<br/>{% api-method-summary %}<br/>
Gets details of referenced schedule.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns the details of the referenced schedule.

<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="reference" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation.
The details of the schedule are returned in the 'resource' field and the 'operation' is set to 'create'.

{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unsuccessful request.
Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'."

{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="put" host="https://api.aedifion.io" path="/v2/datapoint/schedule/{reference}" %}
<br/>{% api-method-summary %}<br/>
Updates the referenced schedule.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Updates the details of the referenced schedule.

<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="reference" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="schedule" type="None" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation.
The details of the schedule are returned in the 'resource' field and the 'operation' is set to 'create'.

{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unsuccessful request.
Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'."

{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="delete" host="https://api.aedifion.io" path="/v2/datapoint/schedule/{reference}" %}
<br/>{% api-method-summary %}<br/>
Delete a schedule.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Deletes a schedule and clears any setpoints that were written while executing the schedule.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="reference" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation.
Since this operation is asynchronous, the caller has to check back that the status of the schedule operation transitions to 'terminated' (success) or 'failed' (error during deletion).
The deleted schedule is returned in the 'resource' field of the result and 'operation' is set to 'delete'.

{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% api-method-response-example httpCode=401 %}
<br/>{% api-method-response-example-description %}
<br/>Unsuccessful request.
Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'."

{% endapi-method-response-example-description %}
<br/>
```


```
{% endapi-method-response-example %}
<br/>{% endapi-method-response %}
<br/>{% endapi-method-spec %}
<br/>{% endapi-method %}
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/components" %}
<br/>{% api-method-summary %}<br/>
Get all available components.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Gets all the available components to be used in a project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. A list of component ids along with their english and german names are returned in the 'resource' field and the 'operation' is set to 'get'.
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
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/component/{component_id}/pins" %}
<br/>{% api-method-summary %}<br/>
Get all pins and its attributes for the component.
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Gets all the defined pins for the component.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="component_id" type="string" required=True%}
<br/>{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% endapi-method-body-parameters %}
<br/>{% endapi-method-request %}
<br/>{% api-method-response %}
<br/>{% api-method-response-example httpCode=200 %}
<br/>{% api-method-response-example-description %}
<br/>Successful operation. A list of pins and its attributes are returned for the component in the 'resource' field and the 'operation' is set to 'get'.
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
<br/>
