# bms-user-controller/getUser

#### 接口简介

  获取用户信息

#### 基本信息：

- 接口状态：已完成
- 接口地址：http://localhost:8000/user/info
- 请求方式：GET
- 请求类型：

#### 请求参数：

| 字段     | 说明 | 类型   | 备注 | 是否必填 |
| -------- | ---- | ------ | ---- | -------- |
| userName | 姓名 | String |      | 是       |

#### 返回参数：

| 字段    | 说明       | 类型   | 备注                       |
| ------- | ---------- | ------ | -------------------------- |
| code    | 接口状态码 | Number | 成功：200  失败：-1        |
| message | 接口信息   | String | 成功：操作成功 <br> 失败： |
| data    | 返回数据   | Object | 是                         |

data：

| 字段       | 说明     | 类型   | 是否非空 | 备注               |
| ---------- | -------- | ------ | -------- | ------------------ |
| id         | 用户id   | String | 是       |                    |
| username   | 用户名   | String | 是       |                    |
| alias      | 用户昵称 | String | 否       |                    |
| avatar     | 头像url  | String | 否       |                    |
| mobile     | 手机号   | Number | 否       |                    |
| bio        | 职业     | String | 是       |                    |
| score      | 积分     | Number | 是       |                    |
| active     | 是否激活 | Number | 是       | 1：是<br/>0：否    |
| status     | 状态     | Number | 是       | 1：使用<br>0：停用 |
| roleId     | 用户角色 | String | 否       |                    |
| createTime | 创建时间 | String | 是       |                    |
| modifyTime | 修改时间 | String | 否       |                    |
| sex        | 性别     | int    | 是       | 1：男，0：女       |

#### 响应实例：

![image-20221128215142568](images\image-20221128215142568.png)