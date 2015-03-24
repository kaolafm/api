##获取指定电台播单列表
===
###请求方式
---

**GET** `http://open.kaolafm.com/v1/radio/playlist?appid={appid}&sign={sign}&openid={openid}&rid={rid}`

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
| rid   | string |   是   |电台id（即接口4当中type为3的cid）
| clockid | string | 否 | 时钟id 第一次不填，之后通过上一次请求返回中的clockId获取
| rate   | string |   否   |音频码率 默认为原始码率，可选值为（32/64/128）




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
| clockId | string	|  时钟id
| hostList.name | string	| 主持人名字
| hostList.description	| string	| 主持人描述
| hostList.img	| string	| 主持人图片




###结果样例
---

    {

    "result": [
        {
            "aid": "1000000768040",
            "cover": "http://image.kaolafm.net/mz/images/201308/63b9f008-a4d0-4856-8113-cff257affc4f/default.jpg",
            "albumId": "1100000000001",
            "albumName": "考拉头条快讯",
            "title": "内蒙古奸杀冤案进入再审程序",
            "playurl": "http://image.kaolafm.net/mz/audios/201411/d584d20f-b336-4f48-af05-fa8e1065e028.mp3?appid=tlvvv4465&carid=100000017370149&audioid=1000000768040",
            "duration": "155965",
            "categoryId": "116",
            "clockId": "103546",
            "intercutTime": "0",
            "hostList": [ ],
            "albumDescription": "",
            "description": "国际国内、社会民生，体育娱乐，一个都不少；时事、政策、新举措，我们始终关注；热门、爆料、奇葩事，我们一直很关心！考拉头条快讯，总有你想听到的"
        },
        {
            "aid": "1000000767726",
            "cover": "http://image.kaolafm.net/mz/images/201409/407dbb2a-7e3a-44ae-a641-05542c6be10c/default.jpg",
            "albumId": "1100000000830",
            "albumName": "考拉假新闻",
            "title": "朝鲜18号鱼塘被金正恩承包",
            "playurl": "http://image.kaolafm.net/mz/audios/201411/04cc2569-a876-4650-a0c0-d64244e25f94.mp3?appid=tlvvv4465&carid=100000017370149&audioid=1000000767726",
            "duration": "78041",
            "categoryId": "116",
            "clockId": "103546",
            "intercutTime": "0",
            "hostList": [ ],
            "albumDescription": "",
            "description": "考拉秉着对新闻求真务实的态度，严肃的说一句：假不假，白玉为堂金做马。\r\n"
        },
        {
            "aid": "1000000761335",
            "cover": null,
            "albumId": "1100000037630",
            "albumName": "2014决战台湾九合一",
            "title": "小百科：柯文哲：深绿医师竞逐台北市长",
            "playurl": "http://image.kaolafm.net/mz/audios/201411/1faea1e4-1548-420b-b242-1da7a9f04753.mp3?appid=tlvvv4465&carid=100000017370149&audioid=1000000761335",
            "duration": "291228",
            "categoryId": "116",
            "clockId": "103546",
            "intercutTime": "0",
            "hostList": [ ],
            "albumDescription": "",
            "description": "凤凰URadio推出“2014决战九合一”特别企划，为你普及九合一选举的基本知识、一手快报现场战况、邀请专家名嘴点评分析、呈现焦点议题的两岸冲突…"
        }
    ],
    "requestId": "tlvvv44651416451775265587"

    }
###错误信息

请参考错误代码释义
