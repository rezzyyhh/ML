# MoneyLion
Technical Assessment :


Please note we will require you to use Java as the language and ideally, Spring Boot as the framework.


User story:
You would like to manage users’ accesses to new features via feature switches,
i.e. enabling/disabling certain feature based on a user’s email and feature names).

Requirements:
# Feature Switches
This is a simple feature switches to manage users' access to new features based on user's email and feature names.

## Available Endpoints
- ```GET /feature?email=XXX&featureName=XXX```  
This endpoint receives `email` (user's email) and `featureName` as request parameters and return the following endpoint.
```
{
  "canAccess": true|false (will be true if the user has accss to the featureName)
}
```

- `POST /feature`  
This endpoint receives the following request in JSON format and returns an empty response
with HTTP Status OK (200) when the database is updated successfully, otherwise return HTTP
Status Not Modifies (304).
```
{
  "feature": "xxx", (string)
  "email": "xxx", (string)
  "enable": true|false (boolean) (uses true to enable a user's access, otherwise false)
}
```
