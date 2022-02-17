# MoneyLion
Technical Assessment :


Please note we will require you to use Java as the language and ideally, Spring Boot as the framework.


User story:
As a Product Manager, you would like to manage users’ accesses to new features via feature switches,
i.e. enabling/disabling certain feature based on a user’s email and feature names).

Requirements:
GET /feature?email=XXX&featureName=XXX
This endpoint receives email (user’s email) and featureName as request parameters and
returns the following response in JSON format.
Example Response:
POST /feature
This endpoint receives the following request in JSON format and returns an empty
response with HTTP Status OK (200) when the database is updated successfully, otherwise
returns H􀂂p Status Not Modified (304).
Example Request:
{
"canAccess": true|false (will be true if the user has access to the featureName
}
{
"featureName": "xxx", (string)
"email": "xxx", (string) (user's name)
"enable": true|false (boolean) (uses true to enable a user's access, otherwise
}
