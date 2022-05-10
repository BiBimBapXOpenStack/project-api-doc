**URL** : `/api/posts/`

**Method** : `PUT`

**Description** : 게시글 수정

**Auth required** : YES

**Request Body**

|Name|Type|Required|Description|example|
|----|----|--------|--------|-------|
|user_id|`BigInt`|`True`|게시글 작성 유저 ID|`"userName"`|
|title|`String`|`True`|게시글 제목|`"Title"`|
|content|`String`|`True`|게시글 본문|`"Lorem Ipsum...."`|
|images|`Array<imageFile>`|`False`|게시글에 포함된 이미지 |`"userName"`|
|imageFile|`Multipartfiel`|`False`|이미지 파일||



## Success Responses

**Condition** : 게시글 수정에 성공

**Code** : `200 OK`

**Content**

```json
{
  "resultCode" : 200,
  "result" : {
      {
        "_id" : "aaa111",
        "user_id" : "userName",
        "createAt" : "Tue May 2 2022 11:00:19 GMT+0900",
        "updateAt" : "Tue May 10 2022 12:12:24 GMT+0900",
      },
  }
}
```

## Failure Response

**Condition** : 권한이 없는 게시글 수정 시도

**Code** : `403 Foribidden`

**Content**

```json
{
  "resultCode" : 403,
  "result" : {
    "errMsg" : "No Permission to current post"
  }
}
```
**Condition** : 수정을 시도하는 게시글이 존재하지 않음

**Code** : `404 Not Found`

**Content**

```json
{
  "resultCode" : 404,
  "result" : {
    "errMsg" : "Post Not Found"
  }
}
```