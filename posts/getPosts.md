**URL** : `/api/posts?page=<pageNumber>`

**Method** : `GET`

**Description** : 게시글 조회

**Auth required** : YES

**Query String**

|Name|Type|Required|Default|Description|example|
|----|----|--------|-------|--------|-------|
|page|`Number`|`True`|0|페이지네이션 인덱스|`1`|

## Success Responses

**Condition** : 게시글 조회에 성공

**Code** : `200 OK`

**Content**

```json
{
  "resultCode" : 200,
  "result" : {
    [
      {
        "_id" : "aaa111",
        "user_id" : "userName",
        "title" : "Post Title",
        "createAt" : "Tue May 2 2022 11:00:19 GMT+0900",
        "updateAt" : "Tue May 10 2022 16:47:29 GMT+0900",
      },
    ]
  }
}
```

## Failure Response

**Condition** : 해당 페이지 인덱스가 존재하지 않을 때

**Code** : `404 Not Found`

**Content**
```json
{
  "resultCode" : 404,
  "result" : { 
    "errMsg" : "Invalid index"
  }
}
```

