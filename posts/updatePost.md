**URL** : `/api/posts/`

**Method** : `PUT`

**Description** : 게시글 수정

**Auth required** : YES

**Request Body**

|Name|Type|Required|Description|example|
|----|----|--------|--------|-------|
|id|`Number`|`True`|게시글 ID|`1`|
|user_id|`Number`|`True`|게시글 작성 유저 ID|`1`|
|title|`String`|`True`|게시글 제목|`"Title"`|
|content|`String`|`True`|게시글 본문|`"Lorem Ipsum...."`|



## Success Responses

**Condition** : 게시글 수정에 성공

**Code** : `200 OK`

