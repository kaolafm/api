##获取电台详情
===
###请求方式
---

**GET** `http://open.kaolafm.com/v1/radio/get?appid={appid}&sign={sign}&openid={openid}&rid={rid}`

###认证参数
---
| 参数名称 | 类型    | 是否必需 |描述
|:------- |-------:|:------:|:----|
| appid   | string |   是   |应用id
| sign    | string |   是   |签名
| openid  | string |   是   |设备标识


###请求参数
---

| 参数名称 | 类型    | 是否必需 |描述
|:------- |-------:|:------:|:----|
| rid   | string |   是   |电台id



###返回参数
---

| 参数名称 | 类型    | 描述 
|:------- |:-------:|:------|
|rid	 | string	 | 电台id
| name	| string	| 电台名称
| description	| string	| 电台描述
| logo | string	| 电台logo
| cover | string | 电台封面
| hostList.name | string	| 主持人名字
| hostList.description	| string	| 主持人描述
| hostList.img	| string	| 主持人图片
|keyWords|string|关键词





###结果样例
---

    {

    "result": {
        "rid": "1200000000099",
        "name": "新闻.fm",
        "description": "考拉新闻，让有趣的人觉得有趣",
        "logo": "http://image.kaolafm.net/mz/images/201411/8b7f476f-7ba9-4d3b-83e7-9b4f32e9b7ce/default.jpg",
        "cover": "http://image.kaolafm.net/mz/images/201411/04ba98db-9774-45b8-a2da-9d74e5b85781/default.jpg",
        "hostList": [ ]
    },
    "requestId": "zcrzd9405141646691769036"

    }

###错误信息

请参考错误代码释义
