**URL** : `/api/members/login`

**Method** : `POST`

**Description** : 사용자 로그인

**Request Body**

|Name|Type|Required|Description|example|
|----|----|--------|-----------|-------|
|email|`String`|`True`|사용자 이메일|`"user@mail.com"`|
|password|`String`|`True`|사용자 비밀번호|`"mypassword123"`|

```json
{
  "email" : "user@mail.com",
  "password" : "mypassword123"
}
```

**Auth required** : NO

## Success Responses

**Condition** : 로그인에 성공

**Code** : `200 OK`

**Content**
```json
{
  "status":"OK",
  "result":
    {
      "id":2,
      "username":"jaemin"
    }
}
```
**Response Headers**
|Name|Type|Description|example|
|----|----|-----------|-------|
|Authorization|`String`|JWT토큰|`"Bearer asnkansd12kld..."`|

## Failure Response

**Condition** : 로그인 실패

**Code** : `400 Bad Request`

**Content**
```json
{
  "status":"BAD_REQUEST",
  "result": "에러메세지"
}
```

