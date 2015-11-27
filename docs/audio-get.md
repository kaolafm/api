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
| rate   | string |   否   |音频码率 默认为原始码率，可选值为（32/64/128）



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
| number	| string	| 期数
| publishDate | String  | 上线日期（毫秒）
| md5   | String  | 文件md5
| rate  | String  | 当前码率
| fileSize | String | 文件大小(字节）
| listenNum | int | 播放次数
| likeNum | int | 点赞数
| commentNum | int | 评论数





###结果样例
---

    {

    "result": {
        "aid": "1000001748680",
        "cover": "http://image.kaolafm.net/mz/images/201508/5d966c83-cc41-41bb-af67-0168b34fe178/default.jpg",
        "albumId": "1100000071593",
        "albumName": "资讯每日评2015",
        "title": "2K屏IUNI U3赶上秋季新机发布浪潮",
        "playurl": "http://image.kaolafm.net/mz/mp3_32/201508/b3dd527a-be6c-4515-9f74-562fc6767ebb.mp3?appid=exvui9434&deviceid=100000034994587&audioid=1000001748680",
        "duration": null,
        "categoryId": "116",
        "clockId": "",
        "intercutTime": "",
        "hostList": [ ],
        "albumDescription": "",
        "description": "2K屏IUNI U3赶上秋季新机发布浪潮",
        "publishDate": "1438744285000",
        "md5": "333333333",
        "rate": "32",
        "number": 1,
        "fileSzie": "222"
    },
    "requestId": "exvui94340.11439350793717116"

}

###错误信息

请参考错误代码释义
