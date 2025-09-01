# User API Spec

## Register User

Endpoint : POST /api/users

Request Body :

````json
{
  "username" : "user123",
  "password" : "secret",
  "name" : "User"
}```

Response Body (Success) :

```json
{
  "data" : {
    "username" : "user123",
    "name" : "User"
  }
}```

Response Body (Failed) :

```json
{
  "errors" : "Username must not blank"
}```

## Login User

Endpoint : POST /api/users/login

Request Body :

```json
{
  "username" : "user123",
  "password" : "secret"
}```

Response Body (Success) :

```json
{
  "data" : {
    "username" : "user123",
    "name" : "User",
    "token" : "token"
  }
}```

Response Body (Failed) :

```json
{
  "errors" : "Username must not blank"
}```

## Get User

Endpoint : GET /api/users/current

Request Header :
- Authorization : token

```json
{
  "data" : {
    "username" : "user123",
    "name" : "User"
  }
}```

## Update User

Endpoint : PATCH /api/users/current

Request Header :
- Authorization : token

Request Body :

```json
{
  "name" : "jika update nama",
  "password" : "jika update password"
}```

## Logout User

Endpoint : DELETE /api/users/current

Request Header :
- Authorization : token

```json
{
  "data" : true
}```
````
