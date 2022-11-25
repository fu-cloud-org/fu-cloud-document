# 福云项目--接口文档
[toc]
## 1	环境变量

### 默认环境1
| 参数名 | 字段值 |
| ------ | ------ |
|baseUrl|http://localhost:8000|


## 2	福云项目--接口文档

##### 说明
> 



##### 联系方式
- **联系人：**
- **邮箱：**
- **网址：**//

##### 文档版本
```
2.0
```


## 3	Bms Comment Cont

## 3.1	getCommentsByPostId

> GET  /comment/commentLists
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|postId||postId|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|array[object]||false||
|⇥ content|string||false||
|⇥ createTime|string||false||
|⇥ id|string||false||
|⇥ postId|string||false||
|⇥ userId|string||false||
|⇥ username|string||false||
| message|string||false||

##### 接口描述
> 




## 3.2	createComment

> POST  /comment/create
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|userId||userId|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| content|string||false||
| postId|string||false||
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|object||false||
|⇥ content|string||false||
|⇥ createTime|string||false||
|⇥ id|string||false||
|⇥ modifyTime|string||false||
|⇥ postId|string||false||
|⇥ userId|string||false||
| message|string||false||

##### 接口描述
> 




## 4	Bms Tag Controll

## 4.1	getPostsByTag

> GET  /tag/{name}
### 地址参数（Path Variable）
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|name||name|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|page||page|
|size||size|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|object||false||
| message|string||false||

##### 接口描述
> 




## 5	Bms Promotion Co

## 5.1	getPromotionList

> GET  /promotion/getAll
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|array[object]||false||
|⇥ description|string||false||
|⇥ id|int32||false||
|⇥ link|string||false||
|⇥ title|string||false||
| message|string||false||

##### 接口描述
> 




## 6	Bms Billboard Co

## 6.1	getNotices

> GET  /billboard/show
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|object||false||
|⇥ content|string||false||
|⇥ createTime|string||false||
|⇥ id|int32||false||
|⇥ show|boolean||false||
| message|string||false||

##### 接口描述
> 




## 7	Bms Tip Controll

## 7.1	getRandomTip

> GET  /tip/daily
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|object||false||
|⇥ author|string||false||
|⇥ content|string||false||
|⇥ id|int32||false||
|⇥ type|boolean||false||
| message|string||false||

##### 接口描述
> 




## 8	Bms Follow Contr

## 8.1	getFans

> GET  /follow/fans/{id}
### 地址参数（Path Variable）
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|id||id|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|username||username|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|array[object]||false||
|⇥ alias|string||false||
|⇥ avatar|string||false||
|⇥ dep|string||false||
|⇥ id|string||false||
|⇥ isMyFollowed|boolean||false||
|⇥ sign|string||false||
|⇥ username|string||false||
| message|string||false||

##### 接口描述
> 




## 8.2	getFollowers

> GET  /follow/followers/{id}
### 地址参数（Path Variable）
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|id||id|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|username||username|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|array[object]||false||
|⇥ alias|string||false||
|⇥ avatar|string||false||
|⇥ dep|string||false||
|⇥ id|string||false||
|⇥ isMyFollowed|boolean||false||
|⇥ sign|string||false||
|⇥ username|string||false||
| message|string||false||

##### 接口描述
> 




## 8.3	handleFollow

> GET  /follow/subscribe/{userId}
### 地址参数（Path Variable）
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|userId||userId|
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|userName||userName|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|object||false||
| message|string||false||

##### 接口描述
> 




## 8.4	handleUnFollow

> GET  /follow/unsubscribe/{userId}
### 地址参数（Path Variable）
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|userId||userId|
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|userName||userName|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|object||false||
| message|string||false||

##### 接口描述
> 




## 8.5	isFollow

> GET  /follow/validate/{postUserId}
### 地址参数（Path Variable）
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|postUserId||postUserId|
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|userName||userName|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|object||false||
| message|string||false||

##### 接口描述
> 




## 9	Ums User Control

## 9.1	getUser

> GET  /user/info
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|userName||userName|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|object||false||
|⇥ active|boolean||false||
|⇥ alias|string||false||
|⇥ avatar|string||false||
|⇥ createTime|string||false||
|⇥ dep|string||false||
|⇥ email|string||false||
|⇥ id|string||false||
|⇥ mobile|string||false||
|⇥ modifyTime|string||false||
|⇥ regional|string||false||
|⇥ roleId|int32||false||
|⇥ score|int32||false||
|⇥ sex|int32||false||
|⇥ sign|string||false||
|⇥ status|boolean||false||
|⇥ username|string||false||
| message|string||false||

##### 接口描述
> 




## 9.2	login

> POST  /user/login
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| password|string||false||
| rememberMe|boolean||false||
| username|string||false||
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|object||false||
| message|string||false||

##### 接口描述
> 




## 9.3	logOut

> GET  /user/logout
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|object||false||
| message|string||false||

##### 接口描述
> 




## 9.4	getProfile

> GET  /user/profile
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|userId||userId|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|object||false||
|⇥ alias|string||false||
|⇥ avatar|string||false||
|⇥ columns|int32||false||
|⇥ commentCount|int32||false||
|⇥ fansCount|int32||false||
|⇥ followerCount|int32||false||
|⇥ id|string||false||
|⇥ postCount|int32||false||
|⇥ sex|int32||false||
|⇥ username|string||false||
| message|string||false||

##### 接口描述
> 




## 9.5	register

> POST  /user/register
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| checkPass|string||false||
| email|string||false||
| name|string||false||
| pass|string||false||
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|object||false||
| message|string||false||

##### 接口描述
> 




## 9.6	updateUser

> POST  /user/update
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| active|boolean||false||
| alias|string||false||
| avatar|string||false||
| createTime|string||false||
| dep|string||false||
| email|string||false||
| id|string||false||
| mobile|string||false||
| modifyTime|string||false||
| regional|string||false||
| roleId|int32||false||
| score|int32||false||
| sex|int32||false||
| sign|string||false||
| status|boolean||false||
| username|string||false||
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|object||false||
|⇥ active|boolean||false||
|⇥ alias|string||false||
|⇥ avatar|string||false||
|⇥ createTime|string||false||
|⇥ dep|string||false||
|⇥ email|string||false||
|⇥ id|string||false||
|⇥ mobile|string||false||
|⇥ modifyTime|string||false||
|⇥ regional|string||false||
|⇥ roleId|int32||false||
|⇥ score|int32||false||
|⇥ sex|int32||false||
|⇥ sign|string||false||
|⇥ status|boolean||false||
|⇥ username|string||false||
| message|string||false||

##### 接口描述
> 




## 9.7	updateAvatar

> GET  /user/updateAvatar
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|avatarPath||avatarPath|
|userName||userName|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|object||false||
| message|string||false||

##### 接口描述
> 




## 9.8	updateAvatar

> POST  /user/uploadAvatar
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|userName||userName|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| file|string||false|file|
### 响应体
● 200 响应数据格式：JSON

##### 接口描述
> 




## 9.9	getUserByName

> GET  /user/{username}
### 地址参数（Path Variable）
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|username||username|
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|pageNo||pageNo|
|size||size|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|object||false||
| message|string||false||

##### 接口描述
> 




## 10	Bms Post Control

## 10.1	view

> GET  /post
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|id||id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|object||false||
| message|string||false||

##### 接口描述
> 




## 10.2	delete

> DELETE  /post/delete/{id}
### 地址参数（Path Variable）
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|id||id|
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|userName||userName|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|string||false||
| message|string||false||

##### 接口描述
> 




## 10.3	getMyPost

> GET  /post/getMyPosts/{id}
### 地址参数（Path Variable）
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|id||id|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|array[object]||false||
|⇥ alias|string||false||
|⇥ avatar|string||false||
|⇥ collects|int32||false||
|⇥ comments|int32||false||
|⇥ cover|string||false||
|⇥ createTime|string||false||
|⇥ essence|boolean||false||
|⇥ id|string||false||
|⇥ modifyTime|string||false||
|⇥ summary|string||false||
|⇥ tags|array[object]||false||
|⇥⇥ id|string||false||
|⇥⇥ name|string||false||
|⇥⇥ postCount|int32||false||
|⇥ title|string||false||
|⇥ top|boolean||false||
|⇥ userId|string||false||
|⇥ username|string||false||
|⇥ view|int32||false||
| message|string||false||

##### 接口描述
> 




## 10.4	list

> GET  /post/list
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|pageNo||pageNo|
|size||size|
|tab||tab|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|object||false||
|⇥ countId|string||false||
|⇥ current|int32||false||
|⇥ maxLimit|int32||false||
|⇥ optimizeCountSql|boolean||false||
|⇥ orders|array[object]||false||
|⇥⇥ asc|boolean||false||
|⇥⇥ column|string||false||
|⇥ pages|int32||false||
|⇥ records|array[object]||false||
|⇥⇥ alias|string||false||
|⇥⇥ avatar|string||false||
|⇥⇥ collects|int32||false||
|⇥⇥ comments|int32||false||
|⇥⇥ cover|string||false||
|⇥⇥ createTime|string||false||
|⇥⇥ essence|boolean||false||
|⇥⇥ id|string||false||
|⇥⇥ modifyTime|string||false||
|⇥⇥ summary|string||false||
|⇥⇥ tags|array[object]||false||
|⇥⇥⇥ id|string||false||
|⇥⇥⇥ name|string||false||
|⇥⇥⇥ postCount|int32||false||
|⇥⇥ title|string||false||
|⇥⇥ top|boolean||false||
|⇥⇥ userId|string||false||
|⇥⇥ username|string||false||
|⇥⇥ view|int32||false||
|⇥ searchCount|boolean||false||
|⇥ size|int32||false||
|⇥ total|int32||false||
| message|string||false||

##### 接口描述
> 




## 10.5	getRecommend

> GET  /post/recommend
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|postId||postId|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|array[object]||false||
|⇥ collects|int32||false||
|⇥ comments|int32||false||
|⇥ content|string||false||
|⇥ cover|string||false||
|⇥ createTime|string||false||
|⇥ essence|boolean||false||
|⇥ id|string||false||
|⇥ modifyTime|string||false||
|⇥ sectionId|int32||false||
|⇥ summary|string||false||
|⇥ title|string||false||
|⇥ top|boolean||false||
|⇥ userId|string||false||
|⇥ view|int32||false||
| message|string||false||

##### 接口描述
> 




## 10.6	release

> POST  /post/release
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|userName||userName|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| content|string||false||
| cover|string||false||
| summary|string||false||
| tags|array[string]||false||
| title|string||false||
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|object||false||
|⇥ collects|int32||false||
|⇥ comments|int32||false||
|⇥ content|string||false||
|⇥ cover|string||false||
|⇥ createTime|string||false||
|⇥ essence|boolean||false||
|⇥ id|string||false||
|⇥ modifyTime|string||false||
|⇥ sectionId|int32||false||
|⇥ summary|string||false||
|⇥ title|string||false||
|⇥ top|boolean||false||
|⇥ userId|string||false||
|⇥ view|int32||false||
| message|string||false||

##### 接口描述
> 




## 10.7	update

> POST  /post/update
### 请求头
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|userName||userName|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| collects|int32||false||
| comments|int32||false||
| content|string||false||
| cover|string||false||
| createTime|string||false||
| essence|boolean||false||
| id|string||false||
| modifyTime|string||false||
| sectionId|int32||false||
| summary|string||false||
| title|string||false||
| top|boolean||false||
| userId|string||false||
| view|int32||false||
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|object||false||
|⇥ collects|int32||false||
|⇥ comments|int32||false||
|⇥ content|string||false||
|⇥ cover|string||false||
|⇥ createTime|string||false||
|⇥ essence|boolean||false||
|⇥ id|string||false||
|⇥ modifyTime|string||false||
|⇥ sectionId|int32||false||
|⇥ summary|string||false||
|⇥ title|string||false||
|⇥ top|boolean||false||
|⇥ userId|string||false||
|⇥ view|int32||false||
| message|string||false||

##### 接口描述
> 




## 10.8	uploadCover

> POST  /post/uploadCover
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|userName||userName|
### 请求体(Request Body)
| 参数名称 | 数据类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| file|string||false|file|
### 响应体
● 200 响应数据格式：JSON

##### 接口描述
> 




## 11	Search Controlle

## 11.1	searchList

> GET  /search
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|keyword||keyword|
|pageNum||pageNum|
|pageSize||pageSize|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|object||false||
|⇥ countId|string||false||
|⇥ current|int32||false||
|⇥ maxLimit|int32||false||
|⇥ optimizeCountSql|boolean||false||
|⇥ orders|array[object]||false||
|⇥⇥ asc|boolean||false||
|⇥⇥ column|string||false||
|⇥ pages|int32||false||
|⇥ records|array[object]||false||
|⇥⇥ alias|string||false||
|⇥⇥ avatar|string||false||
|⇥⇥ collects|int32||false||
|⇥⇥ comments|int32||false||
|⇥⇥ cover|string||false||
|⇥⇥ createTime|string||false||
|⇥⇥ essence|boolean||false||
|⇥⇥ id|string||false||
|⇥⇥ modifyTime|string||false||
|⇥⇥ summary|string||false||
|⇥⇥ tags|array[object]||false||
|⇥⇥⇥ id|string||false||
|⇥⇥⇥ name|string||false||
|⇥⇥⇥ postCount|int32||false||
|⇥⇥ title|string||false||
|⇥⇥ top|boolean||false||
|⇥⇥ userId|string||false||
|⇥⇥ username|string||false||
|⇥⇥ view|int32||false||
|⇥ searchCount|boolean||false||
|⇥ size|int32||false||
|⇥ total|int32||false||
| message|string||false||

##### 接口描述
> 




## 12	Email Controller

## 12.1	getVerifiedCode

> GET  /getCode
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|to||to|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|string||false||
| message|string||false||

##### 接口描述
> 




## 12.2	getVerifiedCode

> POST  /getCode
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|to||to|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|string||false||
| message|string||false||

##### 接口描述
> 




## 12.3	getVerifiedCode

> DELETE  /getCode
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|to||to|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|string||false||
| message|string||false||

##### 接口描述
> 




## 12.4	getVerifiedCode

> PUT  /getCode
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|to||to|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|string||false||
| message|string||false||

##### 接口描述
> 




## 12.5	getVerifiedCode

> PATCH  /getCode
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|to||to|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|string||false||
| message|string||false||

##### 接口描述
> 




## 12.6	getVerifiedCode

> OPTIONS  /getCode
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|to||to|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|string||false||
| message|string||false||

##### 接口描述
> 




## 12.7	getVerifiedCode

> HEAD  /getCode
### 请求参数(Query Param)
| 参数名称 | 默认值 | 描述 |
| ------ | ------ | ------ |
|to||to|
### 响应体
● 200 响应数据格式：JSON
| 参数名称 | 类型 | 默认值 | 不为空 | 描述 |
| ------ | ------ | ------ | ------ | ------ |
| code|int32||false||
| data|string||false||
| message|string||false||

##### 接口描述
> 



