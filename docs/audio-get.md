##获取指定期详情
===
###请求方式
---

**GET** `http://open.kaolafm.com/v1/audio/get?appid={appid}&sign={sign}&openid={openid}&aid={aid}`

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
| aid   | string |   是   |期id



###返回参数
---

| 参数名称 | 类型    | 描述 
|:------- |:-------:|:------|
|id	 | string	 | 期id
| title	| string	| 期标题
| description	| string	| 描述
| albumId | string	| 专辑id
| albumName | string	| 专辑名称
| albumDescription	| string	| 专辑描述
| cover | string	| 封面
| playurl | string	| 播放地址
| duration | string	| 时长 单位秒
| categoryId | string	| 分类id
| clockId | string	|  时钟id
| hostList.name | string	| 主持人名字
| hostList.description	| string	| 主持人描述
| hostList.img	| string	| 主持人图片





###结果样例
---

    {

    "result": {
        "aid": "1000000767984",
        "cover": "http://image.kaolafm.net/mz/images/201401/09ceced2-cb6f-4f41-85ca-cce0e3bdabe1/default.jpg",
        "albumId": "1100000000033",
        "albumName": null,
        "title": "修改防卫合作指针美日各有盘算",
        "playurl": "",
        "duration": null,
        "categoryId": "116",
        "clockId": "",
        "intercutTime": "",
        "hostList": [
            {
                "name": "李红",
                "description": "暂无",
                "img": null
            }
        ],
        "albumDescription": "",
        "description": "日本欲修改日美防卫合作指针应对中国"
    },
    "requestId": "zcrzd9405141646633288338"

    }

###错误信息

请参考错误代码释义