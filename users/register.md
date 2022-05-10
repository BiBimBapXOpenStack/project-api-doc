**URL** : `/api/users/`

**Method** : `POST`

**Description** : 사용자 등록

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

**Condition** : 회원가입에 성공

**Code** : `200 OK`

**Content**
```json
{
  "resultCode" : 200,
  "result" : {
    "username" : "userExample"
  }
}
```

## Failure Response

**Condition** : 이미 존재하는 아이디로 등록을 시도

**Code** : `409 Confilct`

**Content**
```json
{
  "resultCode" : 409,
  "result" : { 
    "errMsg" : "Conflict ID"
  }
}
```

