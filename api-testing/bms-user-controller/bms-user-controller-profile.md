# bms-user-controller/profile

#### 接口简介

&emsp;&emsp;根据用户信息获取用户信息

#### 基本信息：

+ 接口状态：已完成
+ 接口地址：http://localhost:8000/user/profile
+ 请求方式：GET
+ 请求类型：

#### 请求参数：

| 字段 | 说明   | 类型   | 备注 | 是否必填 |
| ---- | ------ | ------ | ---- | -------- |
| id   | 用户id | String | 无   | 是       |

#### 返回参数：

| 字段    | 说明       | 类型   | 备注                         |
| ------- | ---------- | ------ | ---------------------------- |
| code    | 接口状态码 | Number | 成功：200 <br> 失败：无      |
| message | 接口信息   | String | 成功：操作成功 <br> 失败：无 |
| data    | 返回数据   | Object | 是                           |

data：

| 字段          | 说明       | 类型   | 是否非空 | 备注 |
| ------------- | ---------- | ------ | -------- | ---- |
| id            | 用户id     | String | 是       |      |
| username      | 用户名     | String | 是       |      |
| alias         | 用户昵称   | String | 否       |      |
| avatar        | 头像url    | String | 否       |      |
| fansCount     | 关注人数   | Number | 是       |      |
| followerCount | 被关注人数 | Number | 是       |      |
| postCount     | 帖子数量   | Number | 是       |      |
| columns       | 专栏数     | Number | 否       |      |
| commentCount  | 评论数     | Number | 否       |      |

#### 响应实例：

![image-20221122204657506](images\image-20221122204657506.png)

