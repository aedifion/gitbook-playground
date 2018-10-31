# Initial page
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/meta/endpoints" %}
<br/>{% api-method-summary %}<br/>
/v2/meta/endpoints
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
/v2/company
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
/v2/company/roles
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
/v2/company/role
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
<br/>{% api-method-parameter name="role_definition" type="object" required=true%}
<br/>The details of the role to create\n{% endapi-method-parameter %}
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
/v2/company/role/{role_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Updates an existing role for the company.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="role_id" type="integer" required=true%}
<br/>The id of the role.{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="role_definition" type="object" required=true%}
<br/>The details of the role to create\n{% endapi-method-parameter %}
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
/v2/company/role/{role_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Deletes an existing role for this company.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="role_id" type="integer" required=true%}
<br/>The id of the role that should be deleted.{% endapi-method-parameter %}
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
/v2/company/role/{role_id}/user/{user_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Assigns role with its id 'role_id' to user with her/his id 'id'.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="user_id" type="integer" required=true%}
<br/>The unique id of the user{% endapi-method-parameter %}
<br/>{% api-method-parameter name="role_id" type="integer" required=true%}
<br/>The unique id of the role{% endapi-method-parameter %}
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
/v2/company/role/{role_id}/user/{user_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Removes role with id 'role_id' from user with id 'id'.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="user_id" type="integer" required=true%}
<br/>The unique id of the user{% endapi-method-parameter %}
<br/>{% api-method-parameter name="role_id" type="integer" required=true%}
<br/>The unique id of the role{% endapi-method-parameter %}
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
/v2/token
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
<br/>{% api-method-parameter name="validity" type="number"%}
<br/>The validity for the requested token in hours.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="scope" type="string"%}
<br/>The scope of the requested token.{% endapi-method-parameter %}
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
/v2/user
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
<br/>{% api-method-parameter name="user" type="object" required=true%}
<br/>The details of the user to create\n{% endapi-method-parameter %}
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
/v2/user
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
/v2/user
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
<br/>{% api-method-parameter name="user" type="object" required=true%}
<br/>The details of the updated user:{% endapi-method-parameter %}
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
/v2/user
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
/v2/user/resetPassword
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
<br/>{% api-method-parameter name="email" type="string" required=true%}
<br/>The user's email address.{% endapi-method-parameter %}
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
/v2/user/projects
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
/v2/user/favorites
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
/v2/user/plotview
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
<br/>{% api-method-parameter name="plotview" type="object" required=true%}
<br/>The details of the plotview to create.{% endapi-method-parameter %}
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
/v2/user/plotviews
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
/v2/user/plotview/{plotview_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Updates a plotview for this user.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="plotview_id" type="integer" required=true%}
<br/>The id of the plotview to delete{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="plotview" type="object" required=true%}
<br/>The details of the plotview update{% endapi-method-parameter %}
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
/v2/user/plotview/{plotview_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Deletes a plotview for this user.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="plotview_id" type="integer" required=true%}
<br/>The id of the plotview to delete.{% endapi-method-parameter %}
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
/v2/project
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
<br/>{% api-method-parameter name="project" type="object" required=true%}
<br/>The details of the project to create\n{% endapi-method-parameter %}
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
/v2/project/{project_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns the details of the queried project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project that should be retrieved.{% endapi-method-parameter %}
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
/v2/project/{project_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Updates the details of the specified project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project that should be updated.{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="project" type="object" required=true%}
<br/>The details of the update to an existing project:{% endapi-method-parameter %}
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
/v2/project/{project_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Deletes the specified project and all its associated resources.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project that should be deleted.{% endapi-method-parameter %}
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
/v2/project/{project_id}/roles
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns a list of roles defined for the queried project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project.{% endapi-method-parameter %}
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
/v2/project/{project_id}/role
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Creates a new role for this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project.{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="role_definition" type="object" required=true%}
<br/>The details of the role to create\n{% endapi-method-parameter %}
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
/v2/project/{project_id}/role/{role_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Updates an existing role for this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="role_id" type="integer" required=true%}
<br/>The id of the role.{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="role_definition" type="object" required=true%}
<br/>The details of the role to create\n{% endapi-method-parameter %}
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
/v2/project/{project_id}/role/{role_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Deletes an existing role for this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="role_id" type="integer" required=true%}
<br/>The id of the role that should be deleted.{% endapi-method-parameter %}
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
/v2/project/role/{role_id}/user/{user_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Assigns role with its id 'role_id' to user with her/his id 'id'.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="user_id" type="integer" required=true%}
<br/>The unique id of the user{% endapi-method-parameter %}
<br/>{% api-method-parameter name="role_id" type="integer" required=true%}
<br/>The unique id of the role{% endapi-method-parameter %}
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
/v2/project/role/{role_id}/user/{user_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Removes role with id 'role_id' from user with id 'id'.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="user_id" type="integer" required=true%}
<br/>The unique id of the user{% endapi-method-parameter %}
<br/>{% api-method-parameter name="role_id" type="integer" required=true%}
<br/>The unique id of the role{% endapi-method-parameter %}
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
/v2/project/{project_id}/datapointkey
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Creates a new data point key in this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project for which a new data point key should be created.{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="datapointkey" type="object" required=true%}
<br/>The details of the new data point key.{% endapi-method-parameter %}
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
/v2/project/{project_id}/datapointkeys
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns a list of all data point keys that have been created in this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project for which data point keys should be queried.{% endapi-method-parameter %}
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
/v2/project/{project_id}/datapointkey/{datapointkey_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Updates the specified data point key associated with the project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="datapointkey_id" type="integer" required=true%}
<br/>The id of the data point key to update.{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="datapointkey" type="object" required=true%}
<br/>The details of the updated data point key.{% endapi-method-parameter %}
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
/v2/project/{project_id}/datapointkey/{datapointkey_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Deletes the specified data point key from the list of data point keys available in this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="datapointkey_id" type="integer" required=true%}
<br/>The id of the data point key to remove.{% endapi-method-parameter %}
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
/v2/project/{project_id}/datapoints
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns a list of all data points that have been created in this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project for which data points should be queried.{% endapi-method-parameter %}
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
/v2/project/{project_id}/datapoints/favorites
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns a list of all favorite data points that have been created in this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project for which data points should be queried.{% endapi-method-parameter %}
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
/v2/project/{project_id}/datapoints/renamings
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns a list of all data points and their renamings that have been created in this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project for which data points should be queried.{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="datapointkey_id" type="integer" required=true%}
<br/>The id of the datapointkey.{% endapi-method-parameter %}
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
/v2/project/{project_id}/tag
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Creates a new tag that can then be assigned to data points in this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project for which to add a data point tag.{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="tag" type="object" required=true%}
<br/>The details of the tag.{% endapi-method-parameter %}
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
/v2/project/{project_id}/tags
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns a list of all data point tags that have been created in this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project for which to query data point tags.{% endapi-method-parameter %}
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
/v2/project/{project_id}/tag/{tag_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Updates an existing tag associated with this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project for which to update a tag.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="tag_id" type="integer" required=true%}
<br/>The id of the tag to update.{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="tag" type="object" required=true%}
<br/>The details of the updated tag{% endapi-method-parameter %}
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
/v2/project/{project_id}/tag/{tag_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Deletes an existing tag associated with this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project for which to delete a tags.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="tag_id" type="integer" required=true%}
<br/>The id of the tag to delete.{% endapi-method-parameter %}
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
/v2/project/{project_id}/datapoints/byTag
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns a list of all data points by tag that have been initialized in this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project for which to query data points by tag.{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="key" type="string" required=true%}
<br/>The key of the tag.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="value" type="string"%}
<br/>The value of the tag.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="source" type="string"%}
<br/>The source of the tag.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="confirmed" type="string"%}
<br/>The confirmed status of the tag.{% endapi-method-parameter %}
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
<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}/alerts" %}
<br/>{% api-method-summary %}<br/>
/v2/project/{project_id}/alerts
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Returns the details of all alerts in a project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The numeric id of the project for which alerts should be queried.{% endapi-method-parameter %}
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
/v2/project/{project_id}/alert/{alert_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Modify alert settings. For more information on parameters and alarms which can be modified, view the endpoint `/v2/project/{id}/alert` (post).
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The numeric project id for which to edit an alert.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="alert_id" type="integer" required=true%}
<br/>The numeric id of the alert to modify.{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="param" type="string" required=true%}
<br/>The name of the parameter to change.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="value" type="string" required=true%}
<br/>The new value for the specified parameter. Example acceptable values for period are 1s, 5m, 6h, 1w{% endapi-method-parameter %}
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
/v2/project/{project_id}/alert/{alert_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Delete an alert by its ID.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The numeric id of the project for which to delete the specified alert{% endapi-method-parameter %}
<br/>{% api-method-parameter name="alert_id" type="integer" required=true%}
<br/>The numeric id of the alert to delete.{% endapi-method-parameter %}
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
/v2/project/{project_id}/alert/{alert_id}/toggle
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Enable or disable an alert.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The numeric id of the project on which to toggle an alarm.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="alert_id" type="integer" required=true%}
<br/>The numeric id of the alert to toggle.{% endapi-method-parameter %}
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
/v2/project/{project_id}/importTimeseries
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Imports timeseries data defined in a file.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="string" required=true%}
<br/>The id of the project the timeseries belongs to.{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="format" type="string" required=true%}
<br/>The format of the file uploaded.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="on_error" type="string" required=true%}
<br/>Action upon error.{% endapi-method-parameter %}
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
/v2/project/{project_id}/component/
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Adds a new component to the specified project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The numeric id of the project for which to add the new component.{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="component_id" type="integer" required=true%}
<br/>The numeric id of the component to add.{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="component_details" type="object"%}
<br/>The details of the component to add to the project:{% endapi-method-parameter %}
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
/v2/project/{project_id}/component/{componentinproject_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Gets a component defined in project along with its pin details.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The numeric id of the project from which to get a component.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="componentinproject_id" type="integer" required=true%}
<br/>The numeric id of the component to get.{% endapi-method-parameter %}
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
/v2/project/{project_id}/component/{componentinproject_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Edits a component for this project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The numeric id of the project for which to edit a component.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="componentinproject_id" type="integer" required=true%}
<br/>The numeric id of the component to edit.{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="component_details" type="object"%}
<br/>The details of the update to the component.{% endapi-method-parameter %}
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
/v2/project/{project_id}/component/{componentinproject_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Deletes a component defined in the specified project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The numeric id of the project from which to delete a component.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="componentinproject_id" type="integer" required=true%}
<br/>The numeric id of the component to delete.{% endapi-method-parameter %}
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
/v2/project/{project_id}/components
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Get all components that have been added to the project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The numeric id of the project from which to get components.{% endapi-method-parameter %}
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
/v2/project/{project_id}/component/pin/datapoint
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Connects a datapoint to a component's pin within the specified project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project to add datapoint to its component pin.{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="componentinproject_id" type="integer" required=true%}
<br/>**componentinproject_id** [mandatory], the numeric id of the component in the project{% endapi-method-parameter %}
<br/>{% api-method-parameter name="pin_id" type="integer" required=true%}
<br/>**pin_id** [mandatory], the id of the pin.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="dataPointID" type="string" required=true%}
<br/>**dataPointID** [mandatory], the alphanumeric id of the datapoint.{% endapi-method-parameter %}
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
/v2/project/{project_id}/component/pin/datapoint
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Edit a datapoint on component pin for the specified project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project to edit datapoint on its component pin.{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="componentinproject_id" type="integer" required=true%}
<br/>**componentinproject_id** [mandatory], the numeric id of the component in the project{% endapi-method-parameter %}
<br/>{% api-method-parameter name="pin_id" type="integer" required=true%}
<br/>**pin_id** [mandatory], the id of the pin.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="dataPointID" type="string" required=true%}
<br/>**dataPointID** [mandatory], the  alphanumeric id of the datapoint.{% endapi-method-parameter %}
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
/v2/project/{project_id}/component/pin/datapoint
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Deletes a datapoint on component pin defined in project.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project from where to delete the component.{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="componentinproject_id" type="integer" required=true%}
<br/>The id of the component.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="pin_id" type="integer" required=true%}
<br/>The id of the pin.{% endapi-method-parameter %}
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
/v2/datapoint
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
<br/>{% api-method-parameter name="dataPointID" type="string" required=true%}
<br/>The dataPointID of the data point to retrieve.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The numeric id of the project to which the data point identified by _dataPointID_ belongs.{% endapi-method-parameter %}
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
/v2/datapoint
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
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The numeric id of the project.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="dataPointID" type="string" required=true%}
<br/>The alphanumeric identifier of the datapoint.{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="datapoint_details" type="object" required=true%}
<br/>The details of the update to the data point.{% endapi-method-parameter %}
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
/v2/datapoint/timeseries
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
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The id of the project from which to query observations for a data point{% endapi-method-parameter %}
<br/>{% api-method-parameter name="dataPointID" type="string" required=true%}
<br/>Name/ID of the data point, e.g., *bacnet100-4120-CO2*{% endapi-method-parameter %}
<br/>{% api-method-parameter name="start" type="string"%}
<br/>Return only observations *after* this date-time"{% endapi-method-parameter %}
<br/>{% api-method-parameter name="end" type="string"%}
<br/>Return only observations *before* this date-time".{% endapi-method-parameter %}
<br/>{% api-method-parameter name="max" type="integer"%}
<br/>Maximum number of observations to return.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="samplerate" type="string"%}
<br/>Desired sampling rate.{% endapi-method-parameter %}
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
/v2/datapoint/favorite
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
<br/>{% api-method-parameter name="dataPointID" type="string" required=true%}
<br/>The dataPointID to to mark as favorite{% endapi-method-parameter %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The numeric id of the project to which the data point identified by _dataPointID_ belongs{% endapi-method-parameter %}
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
/v2/datapoint/favorite
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
<br/>{% api-method-parameter name="dataPointID" type="string" required=true%}
<br/>The dataPointID of the data point to unset as favorite{% endapi-method-parameter %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The numeric id of the project to which the data point identified by _dataPointID_ belongs{% endapi-method-parameter %}
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
/v2/datapoint/renaming
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
<br/>{% api-method-parameter name="renaming" type="object" required=true%}
<br/>The details of the datapoint renaming.{% endapi-method-parameter %}
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
/v2/datapoint/renaming/{renaming_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Changes the alternative name of a data point under a data point key.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="renaming_id" type="integer" required=true%}
<br/>The id of the data point renaming that should be updated.{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="renaming" type="object" required=true%}
<br/>The details of the data point renaming.{% endapi-method-parameter %}
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
/v2/datapoint/renaming/{renaming_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Deletes the alternative name for the data point referenced by its name/dataPointID under the specified dataPointKey.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="renaming_id" type="integer" required=true%}
<br/>The id of the renaming to delete.{% endapi-method-parameter %}
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
/v2/datapoint/tag
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
<br/>{% api-method-parameter name="dataPointID" type="string" required=true%}
<br/>The dataPointID of the data point to assign a tag to.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The numeric id of the project to which the data point identified by 'dataPointID' belongs to.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="tag_id" type="integer" required=true%}
<br/>The numeric id of the tag which will be assigned to the data point referenced to by 'dataPointID' and 'project_id'.{% endapi-method-parameter %}
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
/v2/datapoint/tag/{tag_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Updates the tag identified by 'id' associated with the data point identified by 'dataPointID' and 'project_id'.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="tag_id" type="integer" required=true%}
<br/>The unique id of the tag to update.{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="dataPointID" type="string" required=true%}
<br/>The dataPointID of the associated data point where the tag will be updated.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The numeric id of the project to which the data point identified by 'dataPointID' belongs to.{% endapi-method-parameter %}
<br/>{% endapi-method-query-parameters %}
<br/>{% api-method-body-parameters %}
<br/>{% api-method-parameter name="tag" type="object" required=true%}
<br/>The details of the updated tag.{% endapi-method-parameter %}
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
/v2/datapoint/tag/{tag_id}
<br/>{% endapi-method-summary %}
<br/>{% api-method-description %}
<br/>Removes the tag identified by 'id' from the data point identified by 'dataPointID' and 'project_id'.
<br/>{% endapi-method-description %}
<br/>{% api-method-spec %}
<br/>{% api-method-request %}
<br/>{% api-method-path-parameters %}
<br/>{% api-method-parameter name="tag_id" type="integer" required=true%}
<br/>The unique id of the tag to delete.{% endapi-method-parameter %}
<br/>{% endapi-method-path-parameters %}
<br/>{% api-method-headers %}
<br/>{% endapi-method-headers %}
<br/>{% api-method-query-parameters %}
<br/>{% api-method-parameter name="dataPointID" type="string" required=true%}
<br/>The dataPointID of the data point from which the tag will be deleted.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The numeric id of the project to which the data point identified by 'dataPointID' belongs to.{% endapi-method-parameter %}
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
/v2/datapoint/setpoint
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
<br/>{% api-method-parameter name="dataPointID" type="string" required=true%}
<br/>The dataPointID of the data point for which to write a setpoint.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="project_id" type="integer" required=true%}
<br/>The numeric id of the project which the data point identified by 'dataPointID' belongs to.{% endapi-method-parameter %}
<br/>{% api-method-parameter name="value" type="string" required=true%}
<br/>The value to write (either a float or 'null' for reset){% endapi-method-parameter %}
<br/>{% api-method-parameter name="priority" type="integer"%}
<br/>
