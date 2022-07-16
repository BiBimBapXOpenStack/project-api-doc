**URL** : `/api/members/signup`

**Method** : `POST`

**Description** : 사용자 등록

**Request Body**

|Name|Type|Required|Description|example|
|----|----|--------|-----------|-------|
|email|`String`|`True`|사용자 이메일|`"user@mail.com"`|
|username|`String`|`True`|사용자 이름|`"userName"`|
|password|`String`|`True`|사용자 비밀번호|`"password"`|

```json
{
  "email" : "user@email.com"
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
  "status" : "OK",
  "result" : 
    {
     "id" : 3,
     "username" : "jaemin"
    }
}
```

## Failure Response

**Condition** : 이미 존재하는 아이디로 등록을 시도

**Code** : `409 Confilct`

**Content**
```json
{
  "status":"CONFLICT",
  "result":"이미 가입되어 있는 유저입니다."
}
```

