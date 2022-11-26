#                        email-controller/getVerifiedCode

#### 接口简介

  获取邮箱验证码

#### 基本信息：

- 接口状态：已完成
- 接口地址：http://localhost:8000/getCode
- 请求方式：GET
- 请求类型：

#### 请求参数：

| 字段 | 说明     | 类型   | 备注       | 是否必填 |
| ---- | -------- | ------ | ---------- | -------- |
| to   | 邮箱账户 | String | 需要已存在 | 是       |

#### 返回参数：

| 字段    | 说明       | 类型   | 备注                           |
| ------- | ---------- | ------ | ------------------------------ |
| code    | 接口状态码 | Number | 成功：200  失败：无            |
| message | 接口信息   | String | 成功：操作成功 <br> 失败：报错 |
| data    | 验证码     | String |                                |

#### 响应实例：

![image-20221124001235683](images\image-20221124001235683.png)