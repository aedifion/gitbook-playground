<<<<<<< HEAD
# Initial page<br/>{% api-method method="get" host="https://api.aedifion.io" path="/v2/meta/endpoints" %}<br/>{% api-method-summary %}
=======
# Initial page
{% api-method method="get" host="https://api.aedifion.io" path="/v2/meta/endpoints" %}
{% api-method-summary %}
>>>>>>> 7f75a6b8758e74914eb477d32f4f24cada760ced
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
<<<<<<< HEAD
{% api-method method="get" host="https://api.aedifion.io" path="/v2/company" %}<br/>{% api-method-summary %}
Get all projects and users defined in the company.
{% endapi-method-summary %}
{% api-method-description %}
Returns a list of projects and users defined for the queried company.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. Returns a list of roles in the queried project.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/company/roles" %}<br/>{% api-method-summary %}
Get all roles defined in the company.
{% endapi-method-summary %}
{% api-method-description %}
Returns a list of roles defined for the queried company.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. Returns a list of roles in the queried company.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="post" host="https://api.aedifion.io" path="/v2/company/role" %}<br/>{% api-method-summary %}
Create a new role for the logged user's company.
{% endapi-method-summary %}
{% api-method-description %}
Creates a new role for the company, user is logged in with.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="role_definition" type="None" required=True%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. Returns details of created role.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'post'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="put" host="https://api.aedifion.io" path="/v2/company/role/{role_id}" %}<br/>{% api-method-summary %}
Updates an existing role for the company.
{% endapi-method-summary %}
{% api-method-description %}
Updates an existing role for the company.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="role_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="role_definition" type="None" required=True%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. Returns details of edited role.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'post'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="delete" host="https://api.aedifion.io" path="/v2/company/role/{role_id}" %}<br/>{% api-method-summary %}
Delete an existing role for the company.
{% endapi-method-summary %}
{% api-method-description %}
Deletes an existing role for this company.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="role_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The deleted project is returned within the 'resource' field and 'operation' will indicate a 'delete' operation
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="post" host="https://api.aedifion.io" path="/v2/company/role/{role_id}/user/{user_id}" %}<br/>{% api-method-summary %}
Assign a role to a user.
{% endapi-method-summary %}
{% api-method-description %}
Assigns role with its id 'role_id' to user with her/his id 'id'.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="user_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="role_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The newly created relation between 'user' and 'role' is returned in the 'resource' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="delete" host="https://api.aedifion.io" path="/v2/company/role/{role_id}/user/{user_id}" %}<br/>{% api-method-summary %}
Removes a role from a user.
{% endapi-method-summary %}
{% api-method-description %}
Removes role with id 'role_id' from user with id 'id'.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="user_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="role_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The deleted relation between 'user' and 'role' is returned in the 'resource' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/token" %}<br/>{% api-method-summary %}
Get authentication token.
{% endapi-method-summary %}
{% api-method-description %}
Returns an authentication token which contains the encrypted user name and password. The token can be used instead of HTTP basic auth by using the token as user name and leaving the password field empty.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% api-method-parameter name="validity" type="number" required=False%}
{% endapi-method-parameter %}
{% api-method-parameter name="scope" type="string" required=False%}
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="post" host="https://api.aedifion.io" path="/v2/user" %}<br/>{% api-method-summary %}
Create a new user.
{% endapi-method-summary %}
{% api-method-description %}
Creates a new user with the specified details.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="user" type="None" required=True%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The newly created user is returned in the 'resource' field and the 'operation' will indicate a CREATE operation.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unsuccessful request. The error is returned in the 'error' field.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/user" %}<br/>{% api-method-summary %}
Get logged in user's details.
{% endapi-method-summary %}
{% api-method-description %}
Returns the details of the logged in user.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="put" host="https://api.aedifion.io" path="/v2/user" %}<br/>{% api-method-summary %}
Update the details of the logged in user.
{% endapi-method-summary %}
{% api-method-description %}
Updates the details of the specified user (specification by authentication credentials).
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="user" type="None" required=True%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="delete" host="https://api.aedifion.io" path="/v2/user" %}<br/>{% api-method-summary %}
CAUTION: Deletes logged in user.
{% endapi-method-summary %}
{% api-method-description %}
Deletes the logged in user and all his/her resources - DANGER to suspend important accounts!
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The deleted user is returned within the 'resource' field and 'operation' will indicate a DELETE operation.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized access.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/user/resetPassword" %}<br/>{% api-method-summary %}
Resets user's password.
{% endapi-method-summary %}
{% api-method-description %}
Triggers a confirmation mail to the given email address that allows to reset user's password. Please also check for the email in your junk mail folder.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% api-method-parameter name="email" type="string" required=True%}
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=404 %}
{% api-method-response-example-description %}
User not found.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=500 %}
{% api-method-response-example-description %}
Out of service.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/user/projects" %}<br/>{% api-method-summary %}
Get user's projects.
{% endapi-method-summary %}
{% api-method-description %}
Returns a list of all projects that the user is authorized for.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. A list of projects that the user is authorized to access is returned.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to get.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/user/favorites" %}<br/>{% api-method-summary %}
Get user's favorite data points.
{% endapi-method-summary %}
{% api-method-description %}
Returns a list of data points that the user marked as his/her favorites.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. A list of all data points that the current user marked as favorites is returned.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to get.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="post" host="https://api.aedifion.io" path="/v2/user/plotview" %}<br/>{% api-method-summary %}
Add a plotview.
{% endapi-method-summary %}
{% api-method-description %}
Creates a new plotview and adds it to the list of plotviews for this user.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="plotview" type="None" required=True%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The user and newly created plotview are returned in the 'resource' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/user/plotviews" %}<br/>{% api-method-summary %}
Get user's plotviews.
{% endapi-method-summary %}
{% api-method-description %}
Returns a list of all plotviews that the user has specified or shared.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. A list of all plotViews for the current user is returned.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to get.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="put" host="https://api.aedifion.io" path="/v2/user/plotview/{plotview_id}" %}<br/>{% api-method-summary %}
Update a plotview.
{% endapi-method-summary %}
{% api-method-description %}
Updates a plotview for this user.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="plotview_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="plotview" type="None" required=True%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The updated plotView is returned in the 'resource' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="delete" host="https://api.aedifion.io" path="/v2/user/plotview/{plotview_id}" %}<br/>{% api-method-summary %}
Delete a plotview.
{% endapi-method-summary %}
{% api-method-description %}
Deletes a plotview for this user.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="plotview_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The newly created plotView is returned in the 'resource' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="post" host="https://api.aedifion.io" path="/v2/project" %}<br/>{% api-method-summary %}
Create a new project.
{% endapi-method-summary %}
{% api-method-description %}
Creates a new project with the specified details.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="project" type="None" required=True%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The newly created project is returned in the 'resource' field and the 'operation' will indicate a CREATE operation.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unsuccessful request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}" %}<br/>{% api-method-summary %}
Get project's details.
{% endapi-method-summary %}
{% api-method-description %}
Returns the details of the queried project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. Returns the project, the company that owns this project, and a list of data point keys associated with this project.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to get.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project_id}" %}<br/>{% api-method-summary %}
Update project's details.
{% endapi-method-summary %}
{% api-method-description %}
Updates the details of the specified project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="project" type="None" required=True%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The updated project is returned within the 'resource' field and 'operation' will indicate a 'update' operation.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/{project_id}" %}<br/>{% api-method-summary %}
Delete project.
{% endapi-method-summary %}
{% api-method-description %}
Deletes the specified project and all its associated resources.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The deleted project is returned within the 'resource' field and 'operation' will indicate a 'delete' operation.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}/roles" %}<br/>{% api-method-summary %}
Get all roles defined in the project.
{% endapi-method-summary %}
{% api-method-description %}
Returns a list of roles defined for the queried project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. Returns a list of roles in the queried project.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/{project_id}/role" %}<br/>{% api-method-summary %}
Create a new role for this project.
{% endapi-method-summary %}
{% api-method-description %}
Creates a new role for this project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="role_definition" type="None" required=True%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. Returns details of created role.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'post'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project_id}/role/{role_id}" %}<br/>{% api-method-summary %}
Updates an existing role for this project.
{% endapi-method-summary %}
{% api-method-description %}
Updates an existing role for this project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="role_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="role_definition" type="None" required=True%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. Returns details of edited role.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'post'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/{project_id}/role/{role_id}" %}<br/>{% api-method-summary %}
Delete an existing role for this project.
{% endapi-method-summary %}
{% api-method-description %}
Deletes an existing role for this project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="role_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The deleted project is returned within the 'resource' field and 'operation' will indicate a 'delete' operation
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/role/{role_id}/user/{user_id}" %}<br/>{% api-method-summary %}
Assign a role to a user.
{% endapi-method-summary %}
{% api-method-description %}
Assigns role with its id 'role_id' to user with her/his id 'id'.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="user_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="role_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The newly created relation between 'user' and 'role' is returned in the 'resource' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/role/{role_id}/user/{user_id}" %}<br/>{% api-method-summary %}
Removes a role from a user.
{% endapi-method-summary %}
{% api-method-description %}
Removes role with id 'role_id' from user with id 'id'.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="user_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="role_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The deleted relation between 'user' and 'role' is returned in the 'resource' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/{project_id}/datapointkey" %}<br/>{% api-method-summary %}
Create new data point key in project.
{% endapi-method-summary %}
{% api-method-description %}
Creates a new data point key in this project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="datapointkey" type="None" required=True%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The newly created data point key is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}/datapointkeys" %}<br/>{% api-method-summary %}
Get list of data point keys associated with project.
{% endapi-method-summary %}
{% api-method-description %}
Returns a list of all data point keys that have been created in this project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project_id}/datapointkey/{datapointkey_id}" %}<br/>{% api-method-summary %}
Updates a data point key.
{% endapi-method-summary %}
{% api-method-description %}
Updates the specified data point key associated with the project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="datapointkey_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="datapointkey" type="None" required=True%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The updated data point key is returned within the 'resource' field and 'operation' will indicate a 'update' operation.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/{project_id}/datapointkey/{datapointkey_id}" %}<br/>{% api-method-summary %}
Deletes a data point key associated with the project.
{% endapi-method-summary %}
{% api-method-description %}
Deletes the specified data point key from the list of data point keys available in this project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="datapointkey_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}/datapoints" %}<br/>{% api-method-summary %}
Get list of data points in this project.
{% endapi-method-summary %}
{% api-method-description %}
Returns a list of all data points that have been created in this project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unsuccessful operation. Details on the error are returned in the 'error' field.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}/datapoints/favorites" %}<br/>{% api-method-summary %}
Get list of favorited data points in this project.
{% endapi-method-summary %}
{% api-method-description %}
Returns a list of all favorite data points that have been created in this project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unsuccessful operation. Details on the error are returned in the 'error' field.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}/datapoints/renamings" %}<br/>{% api-method-summary %}
Get list of data points and their renamings in this project.
{% endapi-method-summary %}
{% api-method-description %}
Returns a list of all data points and their renamings that have been created in this project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% api-method-parameter name="datapointkey_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Success
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unsuccessful operation. Details on the error are returned in the 'error' field.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/{project_id}/tag" %}<br/>{% api-method-summary %}
Create a new tag.
{% endapi-method-summary %}
{% api-method-description %}
Creates a new tag that can then be assigned to data points in this project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="tag" type="None" required=True%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The newly created tag is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}/tags" %}<br/>{% api-method-summary %}
Get all data point tags in this project.
{% endapi-method-summary %}
{% api-method-description %}
Returns a list of all data point tags that have been created in this project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. A list of all tags for data points in the specified project is returned.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project_id}/tag/{tag_id}" %}<br/>{% api-method-summary %}
Update an existing tag.
{% endapi-method-summary %}
{% api-method-description %}
Updates an existing tag associated with this project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="tag_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="tag" type="None" required=True%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The updated tag is returned in the 'resource' field and the 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/{project_id}/tag/{tag_id}" %}<br/>{% api-method-summary %}
Delete a tag.
{% endapi-method-summary %}
{% api-method-description %}
Deletes an existing tag associated with this project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="tag_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The deleted tag is returned in the 'resource' field and the 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}/datapoints/byTag" %}<br/>{% api-method-summary %}
Get all data points in this project with a given tag.
{% endapi-method-summary %}
{% api-method-description %}
Returns a list of all data points by tag that have been initialized in this project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% api-method-parameter name="key" type="string" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="value" type="string" required=False%}
{% endapi-method-parameter %}
{% api-method-parameter name="source" type="string" required=False%}
{% endapi-method-parameter %}
{% api-method-parameter name="confirmed" type="string" required=False%}
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. A list of all data points with the given tag in the specified project is returned.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/{project_id}/alert" %}<br/>{% api-method-summary %}
Create a new alert.
{% endapi-method-summary %}
{% api-method-description %}
Creates a new alert with the specified details. The following parameters can/must be provided:
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

{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="newalert" type="None" required=True%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The newly created alert is returned in the 'resource' field and 'operation' will indicate a 'create' operation.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unsuccessful request. The error is returned in the 'error' field and 'operation' will indicate a 'create' operation.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=415 %}
{% api-method-response-example-description %}
Unsuccessful request. The error is returned in the 'error' field and 'operation' will indicate a 'create' operation.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}/alerts" %}<br/>{% api-method-summary %}
Get all alerts in a project.
{% endapi-method-summary %}
{% api-method-description %}
Returns the details of all alerts in a project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. A list of all alerts for the specified project is returned.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project_id}/alert/{alert_id}" %}<br/>{% api-method-summary %}
Edit an Alert.
{% endapi-method-summary %}
{% api-method-description %}
Modify alert settings. For more information on parameters and alarms which can be modified, view the endpoint `/v2/project/{id}/alert` (post).
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="alert_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% api-method-parameter name="param" type="string" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="value" type="string" required=True%}
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The edited alert is returned in the 'resource' field and the 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/{project_id}/alert/{alert_id}" %}<br/>{% api-method-summary %}
Delete an alert.
{% endapi-method-summary %}
{% api-method-description %}
Delete an alert by its ID.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="alert_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The details of the deleted alarm are returned in the 'resource' field and 'operation' will indicate a 'delete' operation.

{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unsuccessful request.
Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'."

{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project_id}/alert/{alert_id}/toggle" %}<br/>{% api-method-summary %}
Enable or disable an alert.
{% endapi-method-summary %}
{% api-method-description %}
Enable or disable an alert.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="alert_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The toggled alert is returned in the 'resource' field and the 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/{project_id}/importTimeseries" %}<br/>{% api-method-summary %}
Imports timeseries data from a file
{% endapi-method-summary %}
{% api-method-description %}
Imports timeseries data defined in a file.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="string" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% api-method-parameter name="format" type="string" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="on_error" type="string" required=True%}
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The uploaded timeseries is returned in the 'resource' field and the 'operation' will indicate a CREATE operation.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unsuccessful request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/{project_id}/component/" %}<br/>{% api-method-summary %}
Add a new component.
{% endapi-method-summary %}
{% api-method-description %}
Adds a new component to the specified project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% api-method-parameter name="component_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="component_details" type="None" required=False%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The newly added component is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}/component/{componentinproject_id}" %}<br/>{% api-method-summary %}
Get a component for the specified project.
{% endapi-method-summary %}
{% api-method-description %}
Gets a component defined in project along with its pin details.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="componentinproject_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. All component details along with its pin details is returned in the 'resource' field and the 'operation' is set to 'get'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project_id}/component/{componentinproject_id}" %}<br/>{% api-method-summary %}
Edit a component in the specified project.
{% endapi-method-summary %}
{% api-method-description %}
Edits a component for this project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="componentinproject_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="component_details" type="None" required=False%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The edited component is returned in the 'resource' field and the 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/{project_id}/component/{componentinproject_id}" %}<br/>{% api-method-summary %}
Delete a component in the specified project.
{% endapi-method-summary %}
{% api-method-description %}
Deletes a component defined in the specified project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="componentinproject_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The details of the deleted component are returned in the 'resource' field and 'operation' will indicate a 'delete' operation.

{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/project/{project_id}/components" %}<br/>{% api-method-summary %}
Get all components in a project.
{% endapi-method-summary %}
{% api-method-description %}
Get all components that have been added to the project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. A list of component ids along with their english and german names are returned in the 'resource' field and the 'operation' is set to 'get'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="post" host="https://api.aedifion.io" path="/v2/project/{project_id}/component/pin/datapoint" %}<br/>{% api-method-summary %}
Connects a datapoint to a component's pin.
{% endapi-method-summary %}
{% api-method-description %}
Connects a datapoint to a component's pin within the specified project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% api-method-parameter name="componentinproject_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="pin_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="dataPointID" type="string" required=True%}
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The component with added datapoint is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="put" host="https://api.aedifion.io" path="/v2/project/{project_id}/component/pin/datapoint" %}<br/>{% api-method-summary %}
Edits a datapoint on a component pin in the specified project.
{% endapi-method-summary %}
{% api-method-description %}
Edit a datapoint on component pin for the specified project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% api-method-parameter name="componentinproject_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="pin_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="dataPointID" type="string" required=True%}
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The component with edited datapoint is returned in the 'resource' field and the 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="delete" host="https://api.aedifion.io" path="/v2/project/{project_id}/component/pin/datapoint" %}<br/>{% api-method-summary %}
Delete a datapoint on component pin for the project.
{% endapi-method-summary %}
{% api-method-description %}
Deletes a datapoint on component pin defined in project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% api-method-parameter name="componentinproject_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="pin_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The details of the deleted datapoint on component are returned in the 'resource' field and 'operation' will indicate a 'delete' operation.

{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/datapoint" %}<br/>{% api-method-summary %}
Get details about data point.
{% endapi-method-summary %}
{% api-method-description %}
Gets the data point including meta information, i.e., whether it is a user's favorite, its renamings and tags.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% api-method-parameter name="dataPointID" type="string" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The data point including meta information is returned.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="put" host="https://api.aedifion.io" path="/v2/datapoint" %}<br/>{% api-method-summary %}
Change datapoint details.
{% endapi-method-summary %}
{% api-method-description %}
Modifies datapoint details such as safety bounds for setpoints.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="dataPointID" type="string" required=True%}
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="datapoint_details" type="None" required=True%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The modified datapoint is returned in the 'resource' field and the 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/datapoint/timeseries" %}<br/>{% api-method-summary %}
Get the time series data of a data point.
{% endapi-method-summary %}
{% api-method-description %}
Returns the measured time series data for the specified data point
referenced by its name/dataPointID for the time interval specified by **start**
and **end**.
Returns the last (or respectively next) **max** observations, if either **start** nor **end** are provided.

{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="dataPointID" type="string" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="start" type="string" required=False%}
{% endapi-method-parameter %}
{% api-method-parameter name="end" type="string" required=False%}
{% endapi-method-parameter %}
{% api-method-parameter name="max" type="integer" required=False%}
{% endapi-method-parameter %}
{% api-method-parameter name="samplerate" type="string" required=None%}
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. A list of observations for the specified data point is returned.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="post" host="https://api.aedifion.io" path="/v2/datapoint/favorite" %}<br/>{% api-method-summary %}
Set a data point as personal favorite.
{% endapi-method-summary %}
{% api-method-description %}
Sets a data point referenced by its name/dataPointID as a favorite for the user.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% api-method-parameter name="dataPointID" type="string" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The newly created favorite is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unsuccessful operation. Details on the error are returned in the 'error' field.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="delete" host="https://api.aedifion.io" path="/v2/datapoint/favorite" %}<br/>{% api-method-summary %}
Remove a personal favorite data point.
{% endapi-method-summary %}
{% api-method-description %}
Removes a data point from the personal favorites of the user.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% api-method-parameter name="dataPointID" type="string" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The deleted favorite data point is returned in the 'resource' field and the 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="post" host="https://api.aedifion.io" path="/v2/datapoint/renaming" %}<br/>{% api-method-summary %}
Add an alternative name associated with a specific data point key for a data point.
{% endapi-method-summary %}
{% api-method-description %}
Assigns an alternative name to a data point referenced by its name/dataPointID under the specified data point key id.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="renaming" type="None" required=True%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The newly created renaming is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="put" host="https://api.aedifion.io" path="/v2/datapoint/renaming/{renaming_id}" %}<br/>{% api-method-summary %}
Change a renaming.
{% endapi-method-summary %}
{% api-method-description %}
Changes the alternative name of a data point under a data point key.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="renaming_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="renaming" type="None" required=True%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The newly created renaming is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="delete" host="https://api.aedifion.io" path="/v2/datapoint/renaming/{renaming_id}" %}<br/>{% api-method-summary %}
Delete an alternative name for a given data point under a given data point key.
{% endapi-method-summary %}
{% api-method-description %}
Deletes the alternative name for the data point referenced by its name/dataPointID under the specified dataPointKey.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="renaming_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The newly created renaming is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="post" host="https://api.aedifion.io" path="/v2/datapoint/tag" %}<br/>{% api-method-summary %}
Add a tag.
{% endapi-method-summary %}
{% api-method-description %}
Adds a tag to the specified data point.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% api-method-parameter name="dataPointID" type="string" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="tag_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The newly created relation (data point, tag) is returned in the 'resource' field and the 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="put" host="https://api.aedifion.io" path="/v2/datapoint/tag/{tag_id}" %}<br/>{% api-method-summary %}
Update tag associated with data point.
{% endapi-method-summary %}
{% api-method-description %}
Updates the tag identified by 'id' associated with the data point identified by 'dataPointID' and 'project_id'.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="tag_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% api-method-parameter name="dataPointID" type="string" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="tag" type="None" required=True%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation.
The updated tag is returned in the 'resource' field and the 'operation' is set to 'update'.

{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unsuccessful request.
Details on the error are returned in the 'error' field of the response and 'operation' is set to 'update'."

{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="delete" host="https://api.aedifion.io" path="/v2/datapoint/tag/{tag_id}" %}<br/>{% api-method-summary %}
Remove tag from data point.
{% endapi-method-summary %}
{% api-method-description %}
Removes the tag identified by 'id' from the data point identified by 'dataPointID' and 'project_id'.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="tag_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% api-method-parameter name="dataPointID" type="string" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation.
The deleted relation (data point, tag) is returned in the 'resource' field and the 'operation' is set to 'delete'.

{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unsuccessful request.
Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'."

{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="post" host="https://api.aedifion.io" path="/v2/datapoint/setpoint" %}<br/>{% api-method-summary %}
Write a setpoint.
{% endapi-method-summary %}
{% api-method-description %}
Attempts to write 'value' with given 'priority' to the the data point identified by 'dataPointID' and 'project_id'.

This endpoint implements a no-frills, non-acked, stateless, best-effort write service intended for single one-shot setpoint write operations. If you need to write schedules (multiple consecutive setpoints), require acknowledgements, or feedback on the current state of the target datapoint, please refer to `POST/GET/PUT/DELETE /v2/datapoint/schedule`.

**Please note:**
  - Setpoint writing is currently only supported for BACnet.**
  - This endpoint returns '200 - success' if the setpoint operation is authorized and correctly specified. It does not provide any feedback whether the setpoint has actually been written successfully by the remote building network.

{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% api-method-parameter name="dataPointID" type="string" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="value" type="string" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="priority" type="integer" required=None%}
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. The setpoint operation has been triggerd but may still fail on the remote side, i.e., the building network.

{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unsuccessful request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'."

{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="post" host="https://api.aedifion.io" path="/v2/datapoint/schedule" %}<br/>{% api-method-summary %}
Write a schedule of setpoints for given datapoint.
{% endapi-method-summary %}
{% api-method-description %}
 Attempts to write a schedule consisting of different setpoints to the the data point identified by 'dataPointID' and 'project_id'. Returns a unique `reference` for that schedule.
**Note regarding asynchronous communication:**
Since the successful writing of a setpoints in a schedule may require several attempts on the local building network, this api call is asynchronous, i.e., this api call returns *before* the process of writing setpoints in a schedule (and acknowledging it) has been fully concluded. Thus, this api call immediately returns a unique reference that can be used by the caller to query status of this schedule using endpoint `/v2/datapoint/schedule/{id}`.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% api-method-parameter name="dataPointID" type="string" required=True%}
{% endapi-method-parameter %}
{% api-method-parameter name="project_id" type="integer" required=True%}
{% endapi-method-parameter %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="schedule" type="None" required=True%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation.
The details of the schedule created according to this operation is returned in the 'resource' field and the 'operation' is set to 'create'.

{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unsuccessful request.
Details on the error are returned in the 'error' field of the response and 'operation' is set to 'create'."

{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/datapoint/schedule/{reference}" %}<br/>{% api-method-summary %}
Gets details of referenced schedule.
{% endapi-method-summary %}
{% api-method-description %}
Returns the details of the referenced schedule.

{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="reference" type="string" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation.
The details of the schedule are returned in the 'resource' field and the 'operation' is set to 'create'.

{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unsuccessful request.
Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'."

{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="put" host="https://api.aedifion.io" path="/v2/datapoint/schedule/{reference}" %}<br/>{% api-method-summary %}
Updates the referenced schedule.
{% endapi-method-summary %}
{% api-method-description %}
Updates the details of the referenced schedule.

{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="reference" type="string" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% api-method-parameter name="schedule" type="None" required=True%}
{% endapi-method-parameter %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation.
The details of the schedule are returned in the 'resource' field and the 'operation' is set to 'create'.

{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unsuccessful request.
Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'."

{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="delete" host="https://api.aedifion.io" path="/v2/datapoint/schedule/{reference}" %}<br/>{% api-method-summary %}
Delete a schedule.
{% endapi-method-summary %}
{% api-method-description %}
Deletes a schedule and clears any setpoints that were written while executing the schedule.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="reference" type="string" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation.
Since this operation is asynchronous, the caller has to check back that the status of the schedule operation transitions to 'terminated' (success) or 'failed' (error during deletion).
The deleted schedule is returned in the 'resource' field of the result and 'operation' is set to 'delete'.

{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unsuccessful request.
Details on the error are returned in the 'error' field of the response and 'operation' is set to 'delete'."

{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/components" %}<br/>{% api-method-summary %}
Get all available components.
{% endapi-method-summary %}
{% api-method-description %}
Gets all the available components to be used in a project.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. A list of component ids along with their english and german names are returned in the 'resource' field and the 'operation' is set to 'get'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
{% api-method method="get" host="https://api.aedifion.io" path="/v2/component/{component_id}/pins" %}<br/>{% api-method-summary %}
Get all pins and its attributes for the component.
{% endapi-method-summary %}
{% api-method-description %}
Gets all the defined pins for the component.
{% endapi-method-description %}
{% api-method-spec %}
{% api-method-request %}
{% api-method-path-parameters %}
{% api-method-parameter name="component_id" type="string" required=True%}
{% endapi-method-parameter %}
{% endapi-method-path-parameters %}
{% api-method-headers %}
{% endapi-method-headers %}
{% api-method-query-parameters %}
{% endapi-method-query-parameters %}
{% api-method-body-parameters %}
{% endapi-method-body-parameters %}
{% endapi-method-request %}
{% api-method-response %}
{% api-method-response-example httpCode=200 %}
{% api-method-response-example-description %}
Successful operation. A list of pins and its attributes are returned for the component in the 'resource' field and the 'operation' is set to 'get'.
{% endapi-method-response-example-description %}
{% api-method-response-example httpCode=401 %}
{% api-method-response-example-description %}
Unauthorized request. Details on the error are returned in the 'error' field of the response and 'operation' is set to 'get'.
{% endapi-method-response-example-description %}
{% endapi-method-response-example %}
{% endapi-method-spec %}
{% endapi-method %}
=======
>>>>>>> 7f75a6b8758e74914eb477d32f4f24cada760ced
