##获取指定专辑下期列表
===
###请求方式
---

**GET** `http://open.kaolafm.com/v1/audio/list?appid={appid}&sign={sign}&openid={openid}&aid={aid}&page={page}&size={size}`

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
| aid   | string |   是   |专辑id（即接口4当中type为0的cid）
| page    | string |   否   |页数 默认为1
| size | string | 否 | 每页数据条数 默认为10 最大50
| rate   | string |   否   |音频码率 默认为原始码率，可选值为（32/64/128）
| number	| string	| 期数



###返回参数
---

| 参数名称 | 类型    | 描述 
|:------- |:-------:|:------|
|aid	 | string	 | 期id
| title	| string	| 期标题
| description	| string	| 描述
| albumId | string	| 专辑id
| albumName | string	| 专辑名称
| albumDescription	| string	| 专辑描述
| cover | string	| 封面
| playurl | string	| 播放地址
| duration | string	| 时长 单位秒
| categoryId | string	| 分类id
| hostList.name | string	| 主持人名字
| hostList.description	| string	| 主持人描述
| hostList.img	| string	| 主持人图片
| 分页字段
| total	| string	| 记录总数
| prev	| string	| 上一页 无上一页输出 -1
| next	| string	| 下一页 无下一页输出 -1




###结果样例
---

    {

    "result": {
        "total": "392",
        "next": "2",
        "prev": "-1",
        "list": [
            {
                "aid": "1000000767984",
                "cover": "http://image.kaolafm.net/mz/images/201401/09ceced2-cb6f-4f41-85ca-cce0e3bdabe1/default.jpg",
                "albumId": "1100000000033",
                "albumName": "海峡两岸",
                "title": "修改防卫合作指针美日各有盘算",
                "playurl": "http://image.kaolafm.net/mz/audios/201411/1e43462f-319a-4687-a924-fd0b2b08dab2.mp3?appid=zcrzd9405&carid=100000017370142&audioid=1000000767984",
                "duration": "1117192",
                "categoryId": "116",
                "clockId": "",
                "intercutTime": "0",
                "hostList": [ ],
                "albumDescription": "",
                "description": "《海峡两岸》节目分为两个版块：第一个是“热点扫描”，主要报道当日和近期台湾岛内的热点新闻；第二个是“热点透视”，当日或近期涉台热点深度报道"
            },
            {
                "aid": "1000000767983",
                "cover": "http://image.kaolafm.net/mz/images/201401/09ceced2-cb6f-4f41-85ca-cce0e3bdabe1/default.jpg",
                "albumId": "1100000000033",
                "albumName": "海峡两岸",
                "title": "台湾修改食安规定最高罚20亿新台币",
                "playurl": "http://image.kaolafm.net/mz/audios/201411/d4b0f4cb-9ee9-4552-a504-c6457a541ed2.mp3?appid=zcrzd9405&carid=100000017370142&audioid=1000000767983",
                "duration": "71694",
                "categoryId": "116",
                "clockId": "",
                "intercutTime": "0",
                "hostList": [ ],
                "albumDescription": "",
                "description": "《海峡两岸》节目分为两个版块：第一个是“热点扫描”，主要报道当日和近期台湾岛内的热点新闻；第二个是“热点透视”，当日或近期涉台热点深度报道"
            }
                    ]
    },
    "requestId": "zcrzd94051416465975027912"

    }

###错误信息

请参考错误代码释义
