**URL** : `/api/posts/`

**Method** : `POST`

**Description** : 게시글 생성

**Auth required** : YES

**Request Body**

|Name|Type|Required|Description|example|
|----|----|--------|--------|-------|
|user_id|`Number`|`True`|게시글 작성 유저 ID|`1`|
|title|`String`|`True`|게시글 제목|`"Title"`|
|content|`String`|`True`|게시글 본문|`"Lorem Ipsum...."`|
|imageName|`String`|`False`|게시글에 포함된 이미지 이름|`"image1"`|
|file|`file`|`False`|이미지 파일||



## Success Responses

**Condition** : 게시글 생성에 성공

**Code** : `200 OK`

**Content**
