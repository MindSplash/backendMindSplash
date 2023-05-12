| [Документация](../README.md) |
|---|

## Пользователь (UserInfo)

```json
{
  "id": "String",
  "firstName": "String",
  "lastName": "String",
  "login": "String",
  "tasks": [
    {
      "Task"
    }
  ],
  "notes": [
    {
      "Note"
    }
  ]
}
```

## Логин (login)

```json
{
  "id": "String",
  "login": "String",
  "password": "String"
}
```

## API (в дальнейшем переедет в Swagger)
### Get
```
/api/user/info/{id}
```
Параметры:
id - (path) id пользователя (UserInfo)

Response:
```json
{
  "id": "String",
  "firstName": "String",
  "lastName": "String",
  "login": "String",
  "tasks": [
    {
      "Task"
    }
  ],
  "notes": [
    {
      "Note"
    }
  ]
}
```

### Put
```
/api/user/info/update/
```
Request:
```json
{
  "id": "String",
  "firstName": "String",
  "lastName": "String",
  "login": "String",
  "tasks": [
    {
      "Task"
    }
  ],
  "notes": [
    {
      "Note"
    }
  ]
}
```

Response:
```json
{
  "id": "String",
  "status": "String"
}
```

### Post
```
/api/user/login
```
Request:
```json
{
  "login": "String",
  "password": "String"
}
```
Response:
```json
{
  "id": "idUserInfo",
  "status": "String"
}
```
---------------------------------------
```
/api/user/logout
```
Request:
```json
{
  "id": "idUserInfo"
}
```
Response:
```json
{
  "id": "idUserInfo",
  "status": "String"
}
```
---------------------------------------
```
/api/user/register
```
Request:
```json
{
  "id": "String",
  "firstName": "String",
  "lastName": "String",
  "login": "String",
  "tasks": [
    {
      "Task"
    }
  ],
  "notes": [
    {
      "Note"
    }
  ]
}
```
Response:
```json
{
  "id": "idUserInfo",
  "status": "String"
}
```
