**URL** : `/api/posts/?page=<pageNumber>&size=<pageSize>`

**Method** : `GET`

**Description** : 게시글 조회

**Auth required** : YES

**Query String**

|Name|Type|Required|example|Description|
|----|----|--------|--------|-------|
|pageNumber|`Number`|`True`|`0`|페이지네이션 인덱스|
|pageSize|`Number`|`True`|`10`|한 페이지에 가져올 포스트 수|

## Success Responses

**Condition** : 게시글 조회에 성공

**Code** : `200 OK`

**Content**

```json
[
{post 1} , {post 2} ...
]
```
배열안의 각 객체들은 readPost의 content와 동일함

## Failure Response


