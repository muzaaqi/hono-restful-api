# Contact API Spec

## Create Contact

Endpoint : POST /api/contacts

Request Header :

- Authorizaation : token

Request Body :

````json
{
  "first_name" : "Nama Depan",
  "last_name" : "Nama Belakang",
  "email" : "example@email.com",
  "phone" : "+6281234265576"
}```

Response Body :

```json
{
  "data" : {
    "id" : "hjadf-u3y49-uidfh",
    "first_name" : "Nama Depan",
    "last_name" : "Nama Belakang",
    "email" : "example@email.com",
    "phone" : "+6281234265576"
  }
}```

## Get Contact

Endpoint : POST /api/contacts/{idContact}

Request Header :
- Authorizaation : token

Response Body :

```json
{
  "data" : {
    "id" : "hjadf-u3y49-uidfh",
    "first_name" : "Nama Depan",
    "last_name" : "Nama Belakang",
    "email" : "example@email.com",
    "phone" : "+6281234265576"
  }
}```

## Update Contact

Endpoint : PUT /api/contacts

Request Header :
- Authorizaation : token

Request Body :

```json
{
  "first_name" : "Nama Depan",
  "last_name" : "Nama Belakang",
  "email" : "example@email.com",
  "phone" : "+6281234265576"
}```

Response Body :

```json
{
  "data" : {
    "id" : "hjadf-u3y49-uidfh",
    "first_name" : "Nama Depan",
    "last_name" : "Nama Belakang",
    "email" : "example@email.com",
    "phone" : "+6281234265576"
  }
}```

## Remove Contact

Endpoint : DELETE /api/contacts/{idContact}

Request Header :
- Authorizaation : token

Response Body :

```json
{
  "data" : true
}```

## Search Contact

Endpoint : GET /api/contacts

Request Header :
- Authorizaation : token

Query Parameter :
- name : string, search ke first_name / last_name
- email : string, search ke email
- phone : string, search ke phone
- page :  number, default 1
- size : number, default 10

Response Body :

```json
{
  "data" : [
    {
    "id" : "hjadf-u3y49-uidfh",
    "first_name" : "Nama Depan",
    "last_name" : "Nama Belakang",
    "email" : "example@email.com",
    "phone" : "+6281234265576"
    },
    {
    "id" : "hjadf-u3y49-uidfh",
    "first_name" : "Nama Depan",
    "last_name" : "Nama Belakang",
    "email" : "example@email.com",
    "phone" : "+6281234265576"
    }
  ],
  "paging" : {
    "current_page" : 1,
    "total_page" : 10,
    "size" : 10
  }
}```
````
