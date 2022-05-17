**URL** : `/api/posts/<postId>`

**Method** : `DELETE`

**Description** : 특정 게시글 삭제

**Auth required** : YES

**Url Parameter**

|Name|Type|Required|Description|example|
|----|----|--------|--------|-------|
|postId|`String`|`True`|게시글 id|`"aaa111"`|

## Success Responses

**Condition** : 게시글 삭제에 성공

**Code** : `200 OK`

**Content**

```json
{
}
```

## Failure Response

**Condition** : 해당 게시글에 대한 권한이 없을 때

**Code** : `403 Forbidden`

**Content**
```json
{
    "errMsg" : "No permission to current post"
}
```

**Condition** : 해당 게시글이 존재하지 않을 때

**Code** : `404 Not Found`

**Content**
```json
{
    "errMsg" : "Invalid postid"
}
```
