# API Spec

## Authentication


Request :
- Method : POST
- Endpoint : `/api/signup`
- Body :

```json 
{

}
```

## Get Student

Request :
- Method : GET
- Endpoint : `/api/student`

Response :

```json 
{

    "data" : {
         "id" : "string, unique",
         "name" : "string",
         "universitas" : "string",
         "expertise" : "string",
         "skills" : "string"
     }
}
```

## Get Detail Student

Request :
- Method : GET
- Endpoint : `/api/student/:id`

Response :

```json 
{
    "data" : {
         "id" : "string, unique",
         "name" : "string",
         "universitas" : "string",
         "prodi" : "string",
         "expertise" : "string",
         "skills" : "string",
         "deskripsi" : "string",
         "video" : 
     }
}
```

## Update Product

Request :
- Method : PUT
- Endpoint : `/api/products/{id_product}`
- Header :
    - Content-Type: application/json
    - Accept: application/json
- Body :

```json 
{
    "name" : "string",
    "price" : "long",
    "quantity" : "integer"
}
```

Response :

```json 
{
    "code" : "number",
    "status" : "string",
    "data" : {
         "id" : "string, unique",
         "name" : "string",
         "price" : "long",
         "quantity" : "integer",
         "createdAt" : "date",
         "updatedAt" : "date"
     }
}
```

## List Product

Request :
- Method : GET
- Endpoint : `/api/products`
- Header :
    - Accept: application/json
- Query Param :
    - size : number,
    - page : number

Response :

```json 
{
    "code" : "number",
    "status" : "string",
    "data" : [
        {
             "id" : "string, unique",
             "name" : "string",
             "price" : "long",
             "quantity" : "integer",
             "createdAt" : "date",
             "updatedAt" : "date"
        },
        {
             "id" : "string, unique",
             "name" : "string",
             "price" : "long",
             "quantity" : "integer",
             "createdAt" : "date",
             "updatedAt" : "date"
         }
    ]
}
```

## Delete Product

Request :
- Method : DELETE
- Endpoint : `/api/products/{id_product}`
- Header :
    - Accept: application/json

Response :

```json 
{
    "code" : "number",
    "status" : "string"
}
```
