##获取专辑详情
===
###请求方式
---

**GET** `http://open.kaolafm.com/v1/album/get?appid={appid}&sign={sign}&openid={openid}&aid={aid}`

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
| aid   | string |   是   |专辑id


###返回参数
---

| 参数名称 | 类型    | 描述 
|:------- |-------:|:------:|
| aid   | string |   专辑id  |
| name  | string |   专辑名称 |
|cover|string|专辑封面
|description|string|专辑描述
|hostList.name|string|主持人姓名
|hostList.description|string|主持人描述
|hostList.img|string|主持人图片



###结果样例
---

    {

    "result": {
        "aid": "1100000000033",
        "name": "海峡两岸",
        "cover": "http://image.kaolafm.net/mz/images/201401/09ceced2-cb6f-4f41-85ca-cce0e3bdabe1/default.jpg",
        "description": "《海峡两岸》节目分为两个版块：第一个是“热点扫描”，主要报道当日和近期台湾岛内的热点新闻；第二个是“热点透视”，当日或近期涉台热点深度报道",
        "hostList": [
            {
                "name": "桑晨",
                "description": "暂无",
                "img": "http://image.kaolafm.net/mz/images/201401/09ceced2-cb6f-4f41-85ca-cce0e3bdabe1/default.jpg"
            },
            {
                "name": "李红",
                "description": "暂无",
                "img": "http://image.kaolafm.net/mz/images/201401/09ceced2-cb6f-4f41-85ca-cce0e3bdabe1/default.jpg"
            }
        ]
    },
    "requestId": "zcrzd9405141646530105724"

    }

###错误信息

请参考错误代码释义