# bms-follow-controller/follow/validate/{postUserId}-api
#### 接口简介
&emsp;&emsp;验证是否关注目标

#### 基本信息：
+ 接口状态：已完成
+ 接口地址：http://localhost:8000/follow/validate
+ 请求方式：GET
+ 请求类型：
#### 请求参数：
|  字段   | 说明 | 类型 | 备注 | 是否必填 |
|  ----   | ----  | ---- | ---- | ---- |
| postid  | 检查对象id | String | 无 | 是 |
| username  | 我的用户名 | String | 无 | 是 |

#### 相应参数：
|  字段   | 说明 | 类型 | 备注 |
|  ----   | ----  | ---- | ---- | 
| code  | 接口状态码 | Number | 成功：200 | 
| message  | 接口信息 | String | 无 |
|data|返回数据|Object|成功：OK| 

#### 响应实例：
![](image/3-3.png)
