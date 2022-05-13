**URL** : `/api/users/logout`

**Method** : `GET`

**Description** : 사용자 로그아웃

**Header**
|Name|Type|Required|Description|example|
|----|----|--------|-----------|-------|
|X-LoginToken|`String`|`True`|사용자 인증 토큰|`asdT123123ASDTE1245abvTT`|

**Auth required** : YES

## Success Responses

**Condition** : 로그아웃에 성공

**Code** : `204 NO CONTENT`

**Content**
```json
{
}
```

## Failure Response

**Condition** : 유효하지 않은 쿠키 -> 쿠키는 검증 실패시 삭제함

**Code** : `400 Bad Request`

**Content**
```json
{
    "errMsg" : "Invalid Login Token"
}
``

