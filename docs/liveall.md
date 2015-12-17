##获取分类下全部直播列表
===
###请求方式
---

**GET** `http://open.kaolafm.com/v1/live/all?appid={appid}&sign={sign}&openid={openid}&cid={cid}`

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
| cid   | string |   是   |分类id(接口3中cid)



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
	"result": [{
		"id": 1510459361,
		"name": "疯狂直播间",
		"liveName": "疯狂直播间",
		"status": 6,
		"listenNum": 1,
		"likeNum": 0,
		"compereName": "豆苗，小嘎",
		"compereImg": "http://image.kaolafm.net/mz/images/201503/facb3114-a7ce-4828-a151-71238eb4a63e/default.jpg",
		"backImg": "http://image.kaolafm.net/mz/images/201503/facb3114-a7ce-4828-a151-71238eb4a63e/default.jpg",
		"playUrl": "http://play.kaolafm.com/kaolafm/1403264830_1510459361/playlist.m3u8",
		"startTime": 1449745200000,
		"beginTime": "2015-12-10 19:00:00",
		"endTime": "2015-12-10 20:00:00",
		"finishTime": 1449748800000
	}],
	"requestId": "tgdbv86810.11449732692438954"
}

###错误信息

请参考错误代码释义
