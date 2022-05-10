**URL** : `/api/posts/`

**Method** : `POST`

**Description** : 게시글 생성

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

**Condition** : 게시글 생성에 성공

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
      },
  }
}
```
