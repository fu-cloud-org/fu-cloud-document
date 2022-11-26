# bms-promotion-controller/promotion/getAll-api
#### 接口简介
&emsp;&emsp;获取推广列表

#### 基本信息：
+ 接口状态：已完成
+ 接口地址：http://localhost:8000/promotion/getAll
+ 请求方式：GET
+ 请求类型：
#### 请求参数：
&emsp;&emsp;无

#### 相应参数：
|  字段   | 说明 | 类型 | 备注 | 
|  ----   | ----  | ---- | ---- |
| code  | 接口状态码 | Number | 成功：200 |
| message  | 接口信息 | String | 成功：操作成功 |
|data|返回数据|Object||

##### data
|字段|说明|类型|备注|
|-|-|-|-|
|id|推广id|Number||
|title|推广标题|String||
|link|推广链接|String||
|description|推广内容描述|String||

#### 响应实例：
![](5-1.png)
