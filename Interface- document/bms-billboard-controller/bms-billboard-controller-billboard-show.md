# 1.bms-billboard-controller/billboard/show-api
#### 接口简介
&emsp;&emsp;展示

#### 基本信息：
+ 接口状态：已完成
+ 接口地址：http://localhost:8000/billboard/show
+ 请求方式：GET
+ 请求类型：
#### 请求参数：
&emsp;&emsp;无

#### 相应参数：
|  字段   | 说明 | 类型 | 备注 |
|  ----   | ----  | ---- | ---- |
| code  | 接口状态码 | Number | 成功：200 |
| message  | 接口信息 | String | 成功：操作成功     |
|data|  返回数据 | Object| |

##### data
|  字段   | 说明 | 类型 | 备注 |
|  ----   | ----  | ---- | ---- |
| id  | 单元格 | Number | 成功：2 | 
| content  | 文本内容 | String | | 
|createTime|创建时间 | String||
|show|是否展示成功|Boolean|成功：true

#### 响应实例：
<div align=center><img  src="1-1.png"/></div>
