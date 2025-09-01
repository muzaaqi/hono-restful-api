# Address API Spec

## Create Address

Endpoint : POST /api/contacts/{idContact}/addresses

Request Header :

- Authorization : token

Request Body :

````json
{
  "street" : "jalan",
  "city" : "kota",
  "province" : "provinsi",
  "country" : "negara",
  "postal_code" : "21243"
}```

Response Body :

```json
{
  "data" : {
    "id" : "jkhoi-ohdhf-11o44",
    "street" : "jalan",
    "city" : "kota",
    "province" : "provinsi",
    "country" : "negara",
    "postal_code" : "21243"
  }
}```

## Get Address

Endpoint : GET /api/contacts/{idContact}/addresses{idAddress}

Request Header :

- Authorization : token

Response Body :

```json
{
  "data" : {
    "id" : "jkhoi-ohdhf-11o44",
    "street" : "jalan",
    "city" : "kota",
    "province" : "provinsi",
    "country" : "negara",
    "postal_code" : "21243"
  }
}```

## Update Address

Endpoint : PUT /api/contacts/{idContact}/addresses/{idAddress}

Request Header :

- Authorization : token

Request Body :

```json
{
  "street" : "jalan",
  "city" : "kota",
  "province" : "provinsi",
  "country" : "negara",
  "postal_code" : "21243"
}```

Response Body :

```json
{
  "data" : {
    "id" : "jkhoi-ohdhf-11o44",
    "street" : "jalan",
    "city" : "kota",
    "province" : "provinsi",
    "country" : "negara",
    "postal_code" : "21243"
  }
}```

## Remove Address

Endpoint : POST /api/contacts/{idContact}/addresses/{idAddress}

Request Header :

- Authorization : token

Response Body :

```json
{
  "data" : true
}```

## List Address

Endpoint : POST /api/contacts/{idContact}/addresses

Request Header :

- Authorization : token

Response Body :

```json
{
  "data" : [
    {
      "id" : "jkhoi-ohdhf-11o44",
      "street" : "jalan",
      "city" : "kota",
      "province" : "provinsi",
      "country" : "negara",
      "postal_code" : "21243"
    },
    {
      "id" : "jkhoi-ohdhf-11o44",
      "street" : "jalan",
      "city" : "kota",
      "province" : "provinsi",
      "country" : "negara",
      "postal_code" : "21243"
    }.

  ]
}```
````
