##获取传统电台详情接口
===
###请求方式
---

**GET** `http://open.kaolafm.com/v1/broadcast/detail?appid={appid}&sign={sign}&openid={openid}&id={id}`

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
| id   | long |   是   |传统电台id 


###返回参数
---

| 参数名称 | 类型    | 描述 
|:------- |-------:|:------:|
| id   | long | 传统电台id  |
| name  | string |   名称 |
|desc|string|电台描述
|pic|string|电台封面
|playUrl|string|播放url
|classifyId|int|类型
###结果样例
---
```
{
result: {
id: 1600000000510,
name: "央广中国之声",
desc: "中国唯一覆盖全国的24小时新闻直播频率。",
pic: "http://image.kaolafm.net/mz/images/201512/80b53c48-fc67-4ab8-9ebc-a68dc3654419/default.jpg",
playUrl: "http://trslbs.kaolafm.com/016f63815d64d4db/1600000000510/playlist.m3u8",
classifyId: 1,
code: null
},
requestId: "ffzex14032.2331463454842579256"
}
```
