# search-controller/search-api
#### 接口简介
&emsp;&emsp;关键词搜索

#### 基本信息：
+ 接口状态：已完成
+ 接口地址：http://localhost:44444/search
+ 请求方式：GET
+ 请求类型：
#### 请求参数：
|  字段   | 说明 | 类型 | 备注 | 是否必填 |
|  ----   | ----  | ---- | ---- | ---- |
| keyword  | 搜索关键词 | String |  | 是 |


#### 相应参数：
|  字段   | 说明 | 类型 | 备注 | 
|  ----   | ----  | ---- | ---- | 
|  code | 接口状态码 | Number | 成功：200 | 
| message  | 接口信息 | String | 成功：操作成功 |
| data |返回数据|Object||

#### 响应实例：
![](8-1.png)
