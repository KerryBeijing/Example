#黑鸟管理员信息表

----------

##表说明
 * Name：admin_wechat_contact
 * database:wechat
 * platform:MySQL
 * Import:
 * Published:
 * Author:
 * Maintainer:

----------
##结构说明

| 名称        | 类型        | 说明           |
|-------------|-------------|----------------|
| id          | int(11)     |                |
| admin_id    | int(11)     | 管理员id       |
| wechat_id   | varchar(32) | 管理员微信id   |
| nick_name   | varchar(32) | 管理员英文昵称 |
| user_group  | tinyint(4)  |                |
| device_id   | varchar(64) | 设备ID(唯一)   |
| update_time | int(11)     | 更新时间       |
| add_time    | int(11)     | 插入时间       |
| trust       | tinyint(4)  | 托管状态       |

----------
##Example
    `查询黑鸟管理员ID`
     select admin_id from admin_wechat_contact

----------
##Tips
* user_group默认值为0，1代表美小，2代表青少，3代表B2S，4代表成人，5代表达拉斯
* trust 托管状态默认为1，1代表正常，2代表托管
     
    