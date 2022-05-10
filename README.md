# project-api-doc


## Common Error
- [Bad_Request](https://github.com/BiBimBapXOpenStack/project-api-doc/blob/master/common_error/Bad_Request.md)
- [UnAuthorized](https://github.com/BiBimBapXOpenStack/project-api-doc/blob/master/common_error/Unauthorized.md)
## Users
- [register](https://github.com/BiBimBapXOpenStack/project-api-doc/blob/master/users/register.md)
- [login](https://github.com/BiBimBapXOpenStack/project-api-doc/blob/master/users/login.md)
- [logout](https://github.com/BiBimBapXOpenStack/project-api-doc/blob/master/users/logout.md)
## Posts
- [getPost](https://github.com/BiBimBapXOpenStack/project-api-doc/blob/master/posts/getPost.md)
- [getPosts](https://github.com/BiBimBapXOpenStack/project-api-doc/blob/master/posts/getPosts.md)
- [createPost](https://github.com/BiBimBapXOpenStack/project-api-doc/blob/master/posts/createPost.md)
- [updatePost](https://github.com/BiBimBapXOpenStack/project-api-doc/blob/master/posts/updatePost.md)
- [deletePost](https://github.com/BiBimBapXOpenStack/project-api-doc/blob/master/posts/deletePost.md)


## log
- Logback 프레임워크를 사용해서 다양한 레벨(error, warn, info 등) 로 로그 데이터를 남긴다. 만약 try-catch 구문 이용해서 예외 발생 시, error 레벨의 로그를 남겨서 많은 log 데이터에서 보다 쉽게 에러 관련 로그를 구별해낸다.

- 추가적으로, “[POST] api/posts“ API의 경우에는 어떤 유저가 게시글을 올렸는지 혹은 어떤 유저가 게시글을 올리다가 실패했는지를 알기 위해서, user_id 도 찍어내서 로그 데이터를 남기도록 한다.

<img width="566" alt="KakaoTalk_Image_2022-05-10-18-59-46" src="https://user-images.githubusercontent.com/55350092/167603263-4fb6b91a-07a6-4af7-99da-016e3e1f0ce4.png">
