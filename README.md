# Library Apps
Final project upskilled academy

# API Spesification

## Authentication
Request :
- Method : POST
- Endpoint : `/api/authentication`
- Header :
    - Content-Type : application/json
    - Accept : application-json
- Body :

```json
{
    "username" : "string",
    "password" : "string",
}
```

- Response :
```json
{
    "code" : "string",
    "message" : "string",
    "data" : {
        "token" : "string"
    }
}
```
## USER
### Create User
Request :
- Method : POST
- Endpoint : `/api/users`
- Header :
    - Content-Type : application/json
    - Accept : application-json
    - Authorization : Bearer {token}
- Body :

```json
{
    "id" : "string, unique",
    "email" : "string",
    "username" : "string",
    "password" : "string",
    "phone" : "string"
}
```

- Response :
```json
{
    "code" : "string",
    "message" : "string",
    "data" : {
        "id" : "string, unique",
        "email" : "string",
        "username" : "string",
        "phone" : "string",
        "createdAt" : "date"
    }
}
```

### Get User
Request :
- Method : GET
- Endpoint : `/api/users/{id_user}`
- Header :
    - Accept : application-json
    - Authorization : Bearer {token}
- Response :
```json
{
    "code" : "string",
    "message" : "string",
    "data" : {
        "id" : "string, unique",
        "email" : "string",
        "username" : "string",
        "phone" : "string",
        "createdAt" : "date"
    }
}
```

## Borrower
### Create borrower
Request :
- Method : POST
- Endpoint : `/api/borrowers`
- Header :
    - Content-Type : application/json
    - Accept : application-json
    - Authorization : Bearer {token}
- Body :

```json
{
    "id" : "string, unique",
    "name" : "string",
    "email" : "string",
    "phone" : "string",
    "address" : "string"
}
```

- Response :
```json
{
    "code" : "string",
    "message" : "string",
    "data" : {
        "id" : "string, unique",
        "name" : "string",
        "email" : "string",
        "phone" : "string",
        "address" : "string",
        "createdAt" : "date"
    }
}
```

### Get Borrower
Request :
- Method : GET
- Endpoint : `/api/borrowers/{id_borrower}`
- Header :
    - Accept : application-json
    - Authorization : Bearer {token}
- Response :
```json
{
    "code" : "string",
    "message" : "string",
    "data" : {
        "id" : "string, unique",
        "name" : "string",
        "email" : "string",
        "phone" : "string",
        "address" : "string",
        "createdAt" : "date"
    }
}
```