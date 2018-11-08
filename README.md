# Initial page

{% api-method method="get" host="https://api.aedifion.io" path="/v2/meta/endpoints" %}
{% api-method-summary %}
  
 /v2/meta/endpoints   
{% endapi-method-summary %}

{% api-method-description %}
  
Returns a list of available endpoint IDs and their names.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="" type="string" required=false %}

{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. A list of all available endpoint IDs and their names is returned.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to get.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.aedifion.io" path="/v2/company" %}
{% api-method-summary %}
  
 /v2/company   
{% endapi-method-summary %}

{% api-method-description %}
  
Returns a list of projects and users defined for the queried company.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. Returns a list of roles in the queried project.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.aedifion.io" path="/v2/company/roles" %}
{% api-method-summary %}
  
 /v2/company/roles   
{% endapi-method-summary %}

{% api-method-description %}
  
Returns a list of roles defined for the queried company.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. Returns a list of roles in the queried company.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://api.aedifion.io" path="/v2/company/role" %}
{% api-method-summary %}
  
 /v2/company/role   
{% endapi-method-summary %}

{% api-method-description %}
  
Creates a new role for the company, user is logged in with.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="role\_definition" type="object" required=true %}
  
The details of the role to create\n
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. Returns details of created role.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'post'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="put" host="https://api.aedifion.io" path="/v2/company/role/{role\_id}" %}
{% api-method-summary %}
  
 /v2/company/role/{role\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Updates an existing role for the company.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="role\_id" type="integer" required=true %}
  
The id of the role.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter name="role\_definition" type="object" required=true %}
  
The details of the role to create\n
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. Returns details of edited role.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'post'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="delete" host="https://api.aedifion.io" path="/v2/company/role/{role\_id}" %}
{% api-method-summary %}
  
 /v2/company/role/{role\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Deletes an existing role for this company.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="role\_id" type="integer" required=true %}
  
The id of the role that should be deleted.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The deleted project is returned within the 'resource' field and 'operation' will indicate a 'delete' operation
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://api.aedifion.io" path="/v2/company/role/{role\_id}/user/{user\_id}" %}
{% api-method-summary %}
  
 /v2/company/role/{role\_id}/user/{user\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Assigns role with its id 'role\_id' to user with her/his id 'id'.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="user\_id" type="integer" required=true %}
  
The unique id of the user
{% endapi-method-parameter %}

{% api-method-parameter name="role\_id" type="integer" required=true %}
  
The unique id of the role
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The newly created relation between 'user' and 'role' is returned in the 'resource' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="delete" host="https://api.aedifion.io" path="/v2/company/role/{role\_id}/user/{user\_id}" %}
{% api-method-summary %}
  
 /v2/company/role/{role\_id}/user/{user\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Removes role with id 'role\_id' from user with id 'id'.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="user\_id" type="integer" required=true %}
  
The unique id of the user
{% endapi-method-parameter %}

{% api-method-parameter name="role\_id" type="integer" required=true %}
  
The unique id of the role
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The deleted relation between 'user' and 'role' is returned in the 'resource' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.aedifion.io" path="/v2/token" %}
{% api-method-summary %}
  
 /v2/token   
{% endapi-method-summary %}

{% api-method-description %}
  
Returns an authentication token which contains the encrypted user name and password. The token can be used instead of HTTP basic auth by using the token as user name and leaving the password field empty.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="validity" type="number" %}
  
The validity for the requested token in hours.
{% endapi-method-parameter %}

{% api-method-parameter name="scope" type="string" %}
  
The scope of the requested token.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Success
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://api.aedifion.io" path="/v2/user" %}
{% api-method-summary %}
  
 /v2/user   
{% endapi-method-summary %}

{% api-method-description %}
  
Creates a new user with the specified details.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="user" type="object" required=true %}
  
The details of the user to create\n
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The newly created user is returned in the 'resource' field and the 'operation' will indicate a CREATE operation.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unsuccessful request. The error is returned in the 'error' field.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.aedifion.io" path="/v2/user" %}
{% api-method-summary %}
  
 /v2/user   
{% endapi-method-summary %}

{% api-method-description %}
  
Returns the details of the logged in user.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Success
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="put" host="https://api.aedifion.io" path="/v2/user" %}
{% api-method-summary %}
  
 /v2/user   
{% endapi-method-summary %}

{% api-method-description %}
  
Updates the details of the specified user \(specification by authentication credentials\).   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="user" type="object" required=true %}
  
The details of the updated user:
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Success
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="delete" host="https://api.aedifion.io" path="/v2/user" %}
{% api-method-summary %}
  
 /v2/user   
{% endapi-method-summary %}

{% api-method-description %}
  
Deletes the logged in user and all his/her resources - DANGER to suspend important accounts!   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The deleted user is returned within the 'resource' field and 'operation' will indicate a DELETE operation.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized access.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.aedifion.io" path="/v2/user/resetPassword" %}
{% api-method-summary %}
  
 /v2/user/resetPassword   
{% endapi-method-summary %}

{% api-method-description %}
  
Triggers a confirmation mail to the given email address that allows to reset user's password. Please also check for the email in your junk mail folder.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="email" type="string" required=true %}
  
The user's email address.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
  
User not found.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=500 %}
{% api-method-response-example-description %}
  
Out of service.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.aedifion.io" path="/v2/user/projects" %}
{% api-method-summary %}
  
 /v2/user/projects   
{% endapi-method-summary %}

{% api-method-description %}
  
Returns a list of all projects that the user is authorized for.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. A list of projects that the user is authorized to access is returned.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to get.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.aedifion.io" path="/v2/user/favorites" %}
{% api-method-summary %}
  
 /v2/user/favorites   
{% endapi-method-summary %}

{% api-method-description %}
  
Returns a list of data points that the user marked as his/her favorites.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. A list of all data points that the current user marked as favorites is returned.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to get.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://api.aedifion.io" path="/v2/user/plotview" %}
{% api-method-summary %}
  
 /v2/user/plotview   
{% endapi-method-summary %}

{% api-method-description %}
  
Creates a new plotview and adds it to the list of plotviews for this user.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="plotview" type="object" required=true %}
  
The details of the plotview to create.
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The user and newly created plotview are returned in the 'resource' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.aedifion.io" path="/v2/user/plotviews" %}
{% api-method-summary %}
  
 /v2/user/plotviews   
{% endapi-method-summary %}

{% api-method-description %}
  
Returns a list of all plotviews that the user has specified or shared.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. A list of all plotViews for the current user is returned.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to get.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="put" host="https://api.aedifion.io" path="/v2/user/plotview/{plotview\_id}" %}
{% api-method-summary %}
  
 /v2/user/plotview/{plotview\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Updates a plotview for this user.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="plotview\_id" type="integer" required=true %}
  
The id of the plotview to delete
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter name="plotview" type="object" required=true %}
  
The details of the plotview update
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The updated plotView is returned in the 'resource' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="delete" host="https://api.aedifion.io" path="/v2/user/plotview/{plotview\_id}" %}
{% api-method-summary %}
  
 /v2/user/plotview/{plotview\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Deletes a plotview for this user.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="plotview\_id" type="integer" required=true %}
  
The id of the plotview to delete.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The newly created plotView is returned in the 'resource' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://api.aedifion.io" path="/v2/project" %}
{% api-method-summary %}
  
 /v2/project   
{% endapi-method-summary %}

{% api-method-description %}
  
Creates a new project with the specified details.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="project" type="object" required=true %}
  
The details of the project to create\n
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The newly created project is returned in the 'resource' field and the 'operation' will indicate a CREATE operation.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unsuccessful request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project\_id}" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Returns the details of the queried project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project that should be retrieved.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. Returns the project, the company that owns this project, and a list of data point keys associated with this project.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to get.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project\_id}" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Updates the details of the specified project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project that should be updated.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter name="project" type="object" required=true %}
  
The details of the update to an existing project:
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The updated project is returned within the 'resource' field and 'operation' will indicate a 'update' operation.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/{project\_id}" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Deletes the specified project and all its associated resources.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project that should be deleted.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The deleted project is returned within the 'resource' field and 'operation' will indicate a 'delete' operation.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project\_id}/roles" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/roles   
{% endapi-method-summary %}

{% api-method-description %}
  
Returns a list of roles defined for the queried project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. Returns a list of roles in the queried project.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/{project\_id}/role" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/role   
{% endapi-method-summary %}

{% api-method-description %}
  
Creates a new role for this project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter name="role\_definition" type="object" required=true %}
  
The details of the role to create\n
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. Returns details of created role.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'post'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project\_id}/role/{role\_id}" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/role/{role\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Updates an existing role for this project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project.
{% endapi-method-parameter %}

{% api-method-parameter name="role\_id" type="integer" required=true %}
  
The id of the role.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter name="role\_definition" type="object" required=true %}
  
The details of the role to create\n
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. Returns details of edited role.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'post'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/{project\_id}/role/{role\_id}" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/role/{role\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Deletes an existing role for this project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project.
{% endapi-method-parameter %}

{% api-method-parameter name="role\_id" type="integer" required=true %}
  
The id of the role that should be deleted.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The deleted project is returned within the 'resource' field and 'operation' will indicate a 'delete' operation
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/role/{role\_id}/user/{user\_id}" %}
{% api-method-summary %}
  
 /v2/project/role/{role\_id}/user/{user\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Assigns role with its id 'role\_id' to user with her/his id 'id'.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="user\_id" type="integer" required=true %}
  
The unique id of the user
{% endapi-method-parameter %}

{% api-method-parameter name="role\_id" type="integer" required=true %}
  
The unique id of the role
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The newly created relation between 'user' and 'role' is returned in the 'resource' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/role/{role\_id}/user/{user\_id}" %}
{% api-method-summary %}
  
 /v2/project/role/{role\_id}/user/{user\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Removes role with id 'role\_id' from user with id 'id'.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="user\_id" type="integer" required=true %}
  
The unique id of the user
{% endapi-method-parameter %}

{% api-method-parameter name="role\_id" type="integer" required=true %}
  
The unique id of the role
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The deleted relation between 'user' and 'role' is returned in the 'resource' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/{project\_id}/datapointkey" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/datapointkey   
{% endapi-method-summary %}

{% api-method-description %}
  
Creates a new data point key in this project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project for which a new data point key should be created.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter name="datapointkey" type="object" required=true %}
  
The details of the new data point key.
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The newly created data point key is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project\_id}/datapointkeys" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/datapointkeys   
{% endapi-method-summary %}

{% api-method-description %}
  
Returns a list of all data point keys that have been created in this project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project for which data point keys should be queried.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Success
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project\_id}/datapointkey/{datapointkey\_id}" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/datapointkey/{datapointkey\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Updates the specified data point key associated with the project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project.
{% endapi-method-parameter %}

{% api-method-parameter name="datapointkey\_id" type="integer" required=true %}
  
The id of the data point key to update.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter name="datapointkey" type="object" required=true %}
  
The details of the updated data point key.
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The updated data point key is returned within the 'resource' field and 'operation' will indicate a 'update' operation.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/{project\_id}/datapointkey/{datapointkey\_id}" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/datapointkey/{datapointkey\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Deletes the specified data point key from the list of data point keys available in this project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project.
{% endapi-method-parameter %}

{% api-method-parameter name="datapointkey\_id" type="integer" required=true %}
  
The id of the data point key to remove.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Success
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project\_id}/datapoints" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/datapoints   
{% endapi-method-summary %}

{% api-method-description %}
  
Returns a list of all data points that have been created in this project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project for which data points should be queried.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Success
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unsuccessful operation. Details on the error are returned in the 'error' field.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project\_id}/datapoints/favorites" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/datapoints/favorites   
{% endapi-method-summary %}

{% api-method-description %}
  
Returns a list of all favorite data points that have been created in this project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project for which data points should be queried.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Success
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unsuccessful operation. Details on the error are returned in the 'error' field.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project\_id}/datapoints/renamings" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/datapoints/renamings   
{% endapi-method-summary %}

{% api-method-description %}
  
Returns a list of all data points and their renamings that have been created in this project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project for which data points should be queried.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-query-parameters %}
{% api-method-parameter name="datapointkey\_id" type="integer" required=true %}
  
The id of the datapointkey.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Success
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unsuccessful operation. Details on the error are returned in the 'error' field.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/{project\_id}/tag" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/tag   
{% endapi-method-summary %}

{% api-method-description %}
  
Creates a new tag that can then be assigned to data points in this project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project for which to add a data point tag.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter name="tag" type="object" required=true %}
  
The details of the tag.
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The newly created tag is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project\_id}/tags" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/tags   
{% endapi-method-summary %}

{% api-method-description %}
  
Returns a list of all data point tags that have been created in this project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project for which to query data point tags.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. A list of all tags for data points in the specified project is returned.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project\_id}/tag/{tag\_id}" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/tag/{tag\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Updates an existing tag associated with this project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project for which to update a tag.
{% endapi-method-parameter %}

{% api-method-parameter name="tag\_id" type="integer" required=true %}
  
The id of the tag to update.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter name="tag" type="object" required=true %}
  
The details of the updated tag
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The updated tag is returned in the 'resource' field and the 'operation' is set to 'update'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/{project\_id}/tag/{tag\_id}" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/tag/{tag\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Deletes an existing tag associated with this project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project for which to delete a tags.
{% endapi-method-parameter %}

{% api-method-parameter name="tag\_id" type="integer" required=true %}
  
The id of the tag to delete.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The deleted tag is returned in the 'resource' field and the 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project\_id}/datapoints/byTag" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/datapoints/byTag   
{% endapi-method-summary %}

{% api-method-description %}
  
Returns a list of all data points by tag that have been initialized in this project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project for which to query data points by tag.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-query-parameters %}
{% api-method-parameter name="key" type="string" required=true %}
  
The key of the tag.
{% endapi-method-parameter %}

{% api-method-parameter name="value" type="string" %}
  
The value of the tag.
{% endapi-method-parameter %}

{% api-method-parameter name="source" type="string" %}
  
The source of the tag.
{% endapi-method-parameter %}

{% api-method-parameter name="confirmed" type="string" %}
  
The confirmed status of the tag.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. A list of all data points with the given tag in the specified project is returned.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

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

{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project\_id}/alerts" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/alerts   
{% endapi-method-summary %}

{% api-method-description %}
  
Returns the details of all alerts in a project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The numeric id of the project for which alerts should be queried.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. A list of all alerts for the specified project is returned.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project\_id}/alert/{alert\_id}" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/alert/{alert\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Modify alert settings. For more information on parameters and alarms which can be modified, view the endpoint `/v2/project/{id}/alert` \(post\).   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The numeric project id for which to edit an alert.
{% endapi-method-parameter %}

{% api-method-parameter name="alert\_id" type="integer" required=true %}
  
The numeric id of the alert to modify.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-query-parameters %}
{% api-method-parameter name="param" type="string" required=true %}
  
The name of the parameter to change.
{% endapi-method-parameter %}

{% api-method-parameter name="value" type="string" required=true %}
  
The new value for the specified parameter. Example acceptable values for period are 1s, 5m, 6h, 1w
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The edited alert is returned in the 'resource' field and the 'operation' is set to 'update'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/{project\_id}/alert/{alert\_id}" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/alert/{alert\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Delete an alert by its ID.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The numeric id of the project for which to delete the specified alert
{% endapi-method-parameter %}

{% api-method-parameter name="alert\_id" type="integer" required=true %}
  
The numeric id of the alert to delete.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The details of the deleted alarm are returned in the 'resource' field and 'operation' will indicate a 'delete' operation.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unsuccessful request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'."
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project\_id}/alert/{alert\_id}/toggle" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/alert/{alert\_id}/toggle   
{% endapi-method-summary %}

{% api-method-description %}
  
Enable or disable an alert.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The numeric id of the project on which to toggle an alarm.
{% endapi-method-parameter %}

{% api-method-parameter name="alert\_id" type="integer" required=true %}
  
The numeric id of the alert to toggle.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The toggled alert is returned in the 'resource' field and the 'operation' is set to 'update'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/{project\_id}/importTimeseries" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/importTimeseries   
{% endapi-method-summary %}

{% api-method-description %}
  
Imports timeseries data defined in a file.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="string" required=true %}
  
The id of the project the timeseries belongs to.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-query-parameters %}
{% api-method-parameter name="format" type="string" required=true %}
  
The format of the file uploaded.
{% endapi-method-parameter %}

{% api-method-parameter name="on\_error" type="string" required=true %}
  
Action upon error.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The uploaded timeseries is returned in the 'resource' field and the 'operation' will indicate a CREATE operation.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unsuccessful request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/{project\_id}/component/" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/component/   
{% endapi-method-summary %}

{% api-method-description %}
  
Adds a new component to the specified project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The numeric id of the project for which to add the new component.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-query-parameters %}
{% api-method-parameter name="component\_id" type="integer" required=true %}
  
The numeric id of the component to add.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter name="component\_details" type="object" %}
  
The details of the component to add to the project:
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The newly added component is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project\_id}/component/{componentinproject\_id}" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/component/{componentinproject\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Gets a component defined in project along with its pin details.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The numeric id of the project from which to get a component.
{% endapi-method-parameter %}

{% api-method-parameter name="componentinproject\_id" type="integer" required=true %}
  
The numeric id of the component to get.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. All component details along with its pin details is returned in the 'resource' field and the 'operation' is set to 'get'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project\_id}/component/{componentinproject\_id}" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/component/{componentinproject\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Edits a component for this project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The numeric id of the project for which to edit a component.
{% endapi-method-parameter %}

{% api-method-parameter name="componentinproject\_id" type="integer" required=true %}
  
The numeric id of the component to edit.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter name="component\_details" type="object" %}
  
The details of the update to the component.
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The edited component is returned in the 'resource' field and the 'operation' is set to 'update'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/{project\_id}/component/{componentinproject\_id}" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/component/{componentinproject\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Deletes a component defined in the specified project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The numeric id of the project from which to delete a component.
{% endapi-method-parameter %}

{% api-method-parameter name="componentinproject\_id" type="integer" required=true %}
  
The numeric id of the component to delete.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The details of the deleted component are returned in the 'resource' field and 'operation' will indicate a 'delete' operation.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project\_id}/components" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/components   
{% endapi-method-summary %}

{% api-method-description %}
  
Get all components that have been added to the project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The numeric id of the project from which to get components.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. A list of component ids along with their english and german names are returned in the 'resource' field and the 'operation' is set to 'get'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/{project\_id}/component/pin/datapoint" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/component/pin/datapoint   
{% endapi-method-summary %}

{% api-method-description %}
  
Connects a datapoint to a component's pin within the specified project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project to add datapoint to its component pin.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-query-parameters %}
{% api-method-parameter name="componentinproject\_id" type="integer" required=true %}
  
**componentinproject\_id** \[mandatory\], the numeric id of the component in the project
{% endapi-method-parameter %}

{% api-method-parameter name="pin\_id" type="integer" required=true %}
  
**pin\_id** \[mandatory\], the id of the pin.
{% endapi-method-parameter %}

{% api-method-parameter name="dataPointID" type="string" required=true %}
  
**dataPointID** \[mandatory\], the alphanumeric id of the datapoint.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The component with added datapoint is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project\_id}/component/pin/datapoint" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/component/pin/datapoint   
{% endapi-method-summary %}

{% api-method-description %}
  
Edit a datapoint on component pin for the specified project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project to edit datapoint on its component pin.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-query-parameters %}
{% api-method-parameter name="componentinproject\_id" type="integer" required=true %}
  
**componentinproject\_id** \[mandatory\], the numeric id of the component in the project
{% endapi-method-parameter %}

{% api-method-parameter name="pin\_id" type="integer" required=true %}
  
**pin\_id** \[mandatory\], the id of the pin.
{% endapi-method-parameter %}

{% api-method-parameter name="dataPointID" type="string" required=true %}
  
**dataPointID** \[mandatory\], the alphanumeric id of the datapoint.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The component with edited datapoint is returned in the 'resource' field and the 'operation' is set to 'update'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/{project\_id}/component/pin/datapoint" %}
{% api-method-summary %}
  
 /v2/project/{project\_id}/component/pin/datapoint   
{% endapi-method-summary %}

{% api-method-description %}
  
Deletes a datapoint on component pin defined in project.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project from where to delete the component.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-query-parameters %}
{% api-method-parameter name="componentinproject\_id" type="integer" required=true %}
  
The id of the component.
{% endapi-method-parameter %}

{% api-method-parameter name="pin\_id" type="integer" required=true %}
  
The id of the pin.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The details of the deleted datapoint on component are returned in the 'resource' field and 'operation' will indicate a 'delete' operation.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.aedifion.io" path="/v2/datapoint" %}
{% api-method-summary %}
  
 /v2/datapoint   
{% endapi-method-summary %}

{% api-method-description %}
  
Gets the data point including meta information, i.e., whether it is a user's favorite, its renamings and tags.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="dataPointID" type="string" required=true %}
  
The dataPointID of the data point to retrieve.
{% endapi-method-parameter %}

{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The numeric id of the project to which the data point identified by _dataPointID_ belongs.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The data point including meta information is returned.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="put" host="https://api.aedifion.io" path="/v2/datapoint" %}
{% api-method-summary %}
  
 /v2/datapoint   
{% endapi-method-summary %}

{% api-method-description %}
  
Modifies datapoint details such as safety bounds for setpoints.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The numeric id of the project.
{% endapi-method-parameter %}

{% api-method-parameter name="dataPointID" type="string" required=true %}
  
The alphanumeric identifier of the datapoint.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter name="datapoint\_details" type="object" required=true %}
  
The details of the update to the data point.
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The modified datapoint is returned in the 'resource' field and the 'operation' is set to 'update'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="get" host="https://api.aedifion.io" path="/v2/datapoint/timeseries" %}
{% api-method-summary %}
  
 /v2/datapoint/timeseries   
{% endapi-method-summary %}

{% api-method-description %}
  
Returns the measured time series data for the specified data point referenced by its name/dataPointID for the time interval specified by **start** and **end**. Returns the last \(or respectively next\) **max** observations, if either **start** nor **end** are provided.
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The id of the project from which to query observations for a data point
{% endapi-method-parameter %}

{% api-method-parameter name="dataPointID" type="string" required=true %}
  
Name/ID of the data point, e.g., _bacnet100-4120-CO2_
{% endapi-method-parameter %}

{% api-method-parameter name="start" type="string" %}
  
Return only observations _after_ this date-time"
{% endapi-method-parameter %}

{% api-method-parameter name="end" type="string" %}
  
Return only observations _before_ this date-time".
{% endapi-method-parameter %}

{% api-method-parameter name="max" type="integer" %}
  
Maximum number of observations to return.
{% endapi-method-parameter %}

{% api-method-parameter name="samplerate" type="string" %}
  
Desired sampling rate.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. A list of observations for the specified data point is returned.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://api.aedifion.io" path="/v2/datapoint/favorite" %}
{% api-method-summary %}
  
 /v2/datapoint/favorite   
{% endapi-method-summary %}

{% api-method-description %}
  
Sets a data point referenced by its name/dataPointID as a favorite for the user.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="dataPointID" type="string" required=true %}
  
The dataPointID to to mark as favorite
{% endapi-method-parameter %}

{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The numeric id of the project to which the data point identified by _dataPointID_ belongs
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The newly created favorite is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unsuccessful operation. Details on the error are returned in the 'error' field.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="delete" host="https://api.aedifion.io" path="/v2/datapoint/favorite" %}
{% api-method-summary %}
  
 /v2/datapoint/favorite   
{% endapi-method-summary %}

{% api-method-description %}
  
Removes a data point from the personal favorites of the user.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="dataPointID" type="string" required=true %}
  
The dataPointID of the data point to unset as favorite
{% endapi-method-parameter %}

{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The numeric id of the project to which the data point identified by _dataPointID_ belongs
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The deleted favorite data point is returned in the 'resource' field and the 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://api.aedifion.io" path="/v2/datapoint/renaming" %}
{% api-method-summary %}
  
 /v2/datapoint/renaming   
{% endapi-method-summary %}

{% api-method-description %}
  
Assigns an alternative name to a data point referenced by its name/dataPointID under the specified data point key id.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-body-parameters %}
{% api-method-parameter name="renaming" type="object" required=true %}
  
The details of the datapoint renaming.
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The newly created renaming is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="put" host="https://api.aedifion.io" path="/v2/datapoint/renaming/{renaming\_id}" %}
{% api-method-summary %}
  
 /v2/datapoint/renaming/{renaming\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Changes the alternative name of a data point under a data point key.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="renaming\_id" type="integer" required=true %}
  
The id of the data point renaming that should be updated.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter name="renaming" type="object" required=true %}
  
The details of the data point renaming.
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The newly created renaming is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="delete" host="https://api.aedifion.io" path="/v2/datapoint/renaming/{renaming\_id}" %}
{% api-method-summary %}
  
 /v2/datapoint/renaming/{renaming\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Deletes the alternative name for the data point referenced by its name/dataPointID under the specified dataPointKey.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="renaming\_id" type="integer" required=true %}
  
The id of the renaming to delete.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The newly created renaming is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://api.aedifion.io" path="/v2/datapoint/tag" %}
{% api-method-summary %}
  
 /v2/datapoint/tag   
{% endapi-method-summary %}

{% api-method-description %}
  
Adds a tag to the specified data point.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-query-parameters %}
{% api-method-parameter name="dataPointID" type="string" required=true %}
  
The dataPointID of the data point to assign a tag to.
{% endapi-method-parameter %}

{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The numeric id of the project to which the data point identified by 'dataPointID' belongs to.
{% endapi-method-parameter %}

{% api-method-parameter name="tag\_id" type="integer" required=true %}
  
The numeric id of the tag which will be assigned to the data point referenced to by 'dataPointID' and 'project\_id'.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The newly created relation \(data point, tag\) is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="put" host="https://api.aedifion.io" path="/v2/datapoint/tag/{tag\_id}" %}
{% api-method-summary %}
  
 /v2/datapoint/tag/{tag\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Updates the tag identified by 'id' associated with the data point identified by 'dataPointID' and 'project\_id'.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="tag\_id" type="integer" required=true %}
  
The unique id of the tag to update.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-query-parameters %}
{% api-method-parameter name="dataPointID" type="string" required=true %}
  
The dataPointID of the associated data point where the tag will be updated.
{% endapi-method-parameter %}

{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The numeric id of the project to which the data point identified by 'dataPointID' belongs to.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}

{% api-method-body-parameters %}
{% api-method-parameter name="tag" type="object" required=true %}
  
The details of the updated tag.
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The updated tag is returned in the 'resource' field and the 'operation' is set to 'update'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unsuccessful request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'."
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="delete" host="https://api.aedifion.io" path="/v2/datapoint/tag/{tag\_id}" %}
{% api-method-summary %}
  
 /v2/datapoint/tag/{tag\_id}   
{% endapi-method-summary %}

{% api-method-description %}
  
Removes the tag identified by 'id' from the data point identified by 'dataPointID' and 'project\_id'.   
{% endapi-method-description %}

{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="tag\_id" type="integer" required=true %}
  
The unique id of the tag to delete.
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}

{% api-method-query-parameters %}
{% api-method-parameter name="dataPointID" type="string" required=true %}
  
The dataPointID of the data point from which the tag will be deleted.
{% endapi-method-parameter %}

{% api-method-parameter name="project\_id" type="integer" required=true %}
  
The numeric id of the project to which the data point identified by 'dataPointID' belongs to.
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% endapi-method-request %}

{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
  
Successful operation. The deleted relation \(data point, tag\) is returned in the 'resource' field and the 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}

{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
  
Unsuccessful request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'."
{% endapi-method-response-example-description %}

```text

```
{% endapi-method-response-example %}
{% endapi-method-response %}
{% endapi-method-spec %}
{% endapi-method %}

{% api-method method="post" host="https://api.aedifion.io" path="/v2/datapoint/setpoint" %}

