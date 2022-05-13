**URL** : `/api/users/login`

**Method** : `POST`

**Description** : 사용자 로그인

**Request Body**

|Name|Type|Required|Description|example|
|----|----|--------|-----------|-------|
|username|`String`|`True`|사용자 이름|`"userName"`|
|password|`String`|`True`|사용자 비밀번호|`"password"`|

```json
{
  "username" : "example userID",
  "password" : "example password"
}
```

**Auth required** : NO

## Success Responses

**Condition** : 로그인에 성공

**Code** : `200 OK`

**Content**
```json
{
    "username" : "userExample"
}
```

## Failure Response

**Condition** : 로그인 실패

**Code** : `401 Unauthorized`

**Content**
```json
{
    "errMsg" : "Failed to Auth"
}
```

