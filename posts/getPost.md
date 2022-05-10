**URL** : `/api/posts/<postId>`

**Method** : `GET`

**Description** : 특정 게시글 조회

**Auth required** : YES

**Url Parameter**

|Name|Type|Required|Description|example|
|----|----|--------|--------|-------|
|postId|`String`|`True`|게시글 id|`"aaa111"`|

## Success Responses

**Condition** : 게시글 조회에 성공

**Code** : `200 OK`

**Content**

```json
{
  "resultCode" : 200,
  "result" : {
      {
        "_id" : 1,
        "user_id" : 1,
        "username" : "anjm1020",
        "title" : "Post Title",
        "createAt" : "Tue May 2 2022 11:00:19 GMT+0900",
        "updateAt" : "Tue May 10 2022 16:47:29 GMT+0900",
      },
  }
}
```

## Failure Response

**Condition** : 해당 게시글이 존재하지 않을 때

**Code** : `404 Not Found`

**Content**
```json
{
  "resultCode" : 404,
  "result" : { 
    "errMsg" : "Invalid postid"
  }
}
```
