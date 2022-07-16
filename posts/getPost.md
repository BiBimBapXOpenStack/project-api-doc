**URL** : `/api/posts/<postId>`

**Method** : `GET`

**Description** : 특정 게시글 조회

**Auth required** : YES

**Url Parameter**

|Name|Type|Required|Description|example|
|----|----|--------|--------|-------|
|postId|`Long`|`True`|게시글 id|`"1"`|

## Success Responses

**Condition** : 게시글 조회에 성공

**Code** : `200 OK`

**Content**

```json
{
  "id":1,
  "title" : "admin post",
  "content":"admin body asdasdas",
  "imageId":2,
  "imageUrl":"https://api-storage.cloud.toast.com/v1/AUTH_35682dae0076479ab712dbb328468535/ajm-test/1657608859095/2A342087-BC2B-4823-8CEB-F63097013FA9_1_201_a.jpeg",
  "userId":1,
  "username":"admin"
}
```

|Name|Type|Description|example|
|----|----|--------|-------|
|id|`Long`|게시글 id|`1`|
|title|`String`|게시글 title|`"post title"`|
|content|`String`|게시글 본문|`"post body ..."`|
|imageId|`Long`|게시글 이미지 id|`1`|
|imageUrl|`String`|게시글 이미지 엔드포인트|`"https://api-storgae...."`|
|userId|`Long`|게시글 작성자 id|`1`|
|username|`String`|게시글 작성자 이름|`"jaemin"`|

## Failure Response

