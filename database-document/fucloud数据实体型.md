* bms_billboard 公告
  
| 字段名称 | 类型 | 说明 |
| :-----| :---- | :-----|
|  id    |  int    |  公告编号      |
| content | varchar(255) | 公告内容 |
| create_time | datetime | 公告日期 | 
| show | tinyint(1) | 0\|1,是否处于展示中 |


* bms_follow 关注
  
| 字段名称 | 类型 | 说明 |
| :-----| :---- | :-----|
| id | int | 编号 |
| parent_id | varchar(20) | 被关注者id|
|follower_id | varchar(20) | 粉丝id | 

* bms_post 帖子
  
| 字段名称 | 类型 | 说明 |
| :-----| :---- | :-----|
| id | varchar(20) | 帖子编号 | 
| title | varchar(255) | 标题 | 
| content | longtext character | 内容 | 
| user_id | varchar(20) | 作者编号 | 
| comments | int | 评论数|
| collects | int | 收藏数|
| view | int | 浏览数 |
| top | bit(1) | 是否置顶 | 
| essence | bit(1) | 是否为精华贴 |
| section_id | int | 问答id | 
| create_time | datetime  | 发布时间 |
| modify_time | datetime | 修改时间 | 
| cover | varchar(1000) | 封面 | 
| summary | longtext | 简介 | 


* bms_comment 评论 

| 字段名称 | 类型 | 说明 |
| :-----| :---- | :-----|
| id | varchar(20) | 评论编号 |
| content | varchar(1000) | 评论内容 | 
| user_id | varchar(20) | 作者ID | 
| post_id | varchar(20) | 帖子ID |
| create_time | datetime | 发布时间 |
| modify_time | datetime | 修改时间 | 

* bms_tag 标签 

| 字段名称 | 类型 | 说明 |
| :-----| :---- | :-----|
| id | varchar(20) | 标签编号 |
| name | varchar(255) | 标签名 |
| post_count | int | 关联帖子数 | 


* bms_post_tag 帖子-标签

| 字段名称 | 类型 | 说明 |
| :-----| :---- | :-----|
| id | int | 编号 | 
| tag_id | varchar(20) | 标签编号 | 
| post_id | varchar(20) | 帖子编号 |

* bms_promotion 推广

| 字段名称 | 类型 | 说明 |
| :-----| :---- | :-----|
| id | int | 编号 | 
| title | varchar(255) | 标题 | 
| link | varchar(255)| 链接 | 
| description | varchar(255) | 说明 | 

* bms_tip 赠言

| 字段名称 | 类型 | 说明 |
| :-----| :---- | :-----|
| id | int | 编号 | 
| content | varchar(1000) | 内容 |
| author | varchar(50) | 作者 | 
| type | tinyint | 是否过期 | 


* ums_user 用户

| 字段名称 | 类型 | 说明 |
| :-----| :---- | :-----|
| id | varchar(20) | 编号 |
| username | varchar(15) | 用户名 |
| alias | varchar(255) | 用户昵称 | 
|password | varchar(100) | 密码 |
| avatar |  varchar(1000) | 头像 |
| email |varchar(255) | 邮箱 |
| mobile | varchar(255) | 电话号码 |
| score |int |积分 |
| token | varchar(255) | token|
| bio |  varchar(255) | 个人简介 |
| active | bit(1) | 是否激活|
| status |  bit(1) | 状态 |
| role_id | int | 用户角色 |
| create_time |  datetime | 加入时间 |
| modify_time |  datetime | 修改时间 |
