**URL** : `/api/users/logout`

**Method** : `GET`

**Description** : 사용자 로그아웃

**Header**
|Name|Type|Required|Description|example|
|----|----|--------|-----------|-------|
|loginToken|`String`|`True`|사용자 인증 토큰|`asdT123123ASDTE1245abvTT`|

**Request Body**

<!-- 
|Name|Type|Required|Description|example|
|----|----|--------|-----------|-------|
|username|`String`|`True`|사용자 이름|`"userName"`|
|password|`String`|`True`|사용자 비밀번호|`"password"`| 
-->

<!-- 
```json
{
  "username" : "example userID",
  "password" : "example password"
}
``` -->

**Auth required** : YES

## Success Responses

**Condition** : 로그아웃에 성공

**Code** : `200 OK`

**Content**
```json
{
  "resultCode" : 200,
  "result" : {}
}
```

## Failure Response

**Condition** : 유효하지 않은 쿠키 -> 쿠키는 검증 실패시 삭제함

**Code** : `400 Bad Request`

**Content**
```json
{
  "resultCode" : 400,
  "result" : { 
    "errMsg" : "Invalid Login Token"
  }
}
```

**Condition** : 로그인하지 않은 사용자가 로그아웃을 시도

**Code** : `401 Unauthorized`

**Content**
```json
{
  "resultCode" : 401,
  "result" : { 
    "errMsg" : "Unauthroized User tried to logout"
  }
}
```

