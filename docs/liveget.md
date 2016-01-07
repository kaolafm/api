##获取直播详情
===
###请求方式
---

**GET** `http://open.kaolafm.com/v1/live/get?appid={appid}&sign={sign}&openid={openid}&liveId={liveId}`

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
| liveId   | string |   是   |计划id（直播列表接口中返回的id）



###返回参数
---

| 参数名称 | 类型    | 描述 
|:------- |:-------:|:------|
|id	|Long	|计划id |
|name	|string	|直播名称|
|liveName |string|	所属直播电台名称|
|status	|Integer|	直播状态（0:已经结束,1:直播中,6未开播 7 已延期）|
|listenNum| Integer|	收听人数|
|likeNum|Integer|	赞数|
|compereName|	string|	主播名称|
|compereImg|	string|	主播头像|
|backImg|	string|	封面图片|
|playUrl|	string|	直播地址|
|startTime|	Long  |开始时间 毫秒|	
|finishTime|	Long |结束时间 毫秒|
|beginTime|	String|  开始时间 日期格式|
|endTime|	String|	结束时间 日期格式|





###结果样例
---
{
	"result": {
		"id": 1567564270,
		"name": "金荣时间",
		"liveName": "金荣时间",
		"status": 7,
		"listenNum": 6,
		"likeNum": 90,
		"compereName": "金荣",
		"compereImg": "http://image.kaolafm.net/mz/images/201509/7fa75ec0-d89d-46f5-8869-0d6f28ff4f32/default.jpg",
		"backImg": "http://image.kaolafm.net/mz/images/201509/7fa75ec0-d89d-46f5-8869-0d6f28ff4f32/default.jpg",
		"playUrl": "http://play.kaolafm.com/kaolafm/1444117418_1567564270/playlist.m3u8",
		"startTime": 1452133800000,
		"beginTime": "2016-01-07 10:30:00",
		"endTime": "2016-01-07 20:05:00",
		"finishTime": 1452168300000
	},
	"requestId": "ffzex14030.11452150614025428"
}

###错误信息

请参考错误代码释义
