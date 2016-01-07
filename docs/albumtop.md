##获取指定分类下专辑点击top50
===
###请求方式
---

**GET** `http://open.kaolafm.com/v1/album/top?appid={appid}&sign={sign}&openid={openid}`

###认证参数
---
| 参数名称 | 类型    | 是否必需 |描述
|:------- |-------:|:------:|:----|
| appid   | string |   是   |应用id
| sign    | string |   是   |签名
| openid  | string |   是   |设备标识


###返回参数
---

| 参数名称 | 类型    | 描述 
|:------- |-------:|:------:|
| cid   | string |   内容id  |
| type    | string |   内容类型(0:专辑  )   |
| name  | string |   名称 |
|img|string|封面
|description|string|内容描述
|categoryId|string|分类id
|categoryName|string|分类名称
|分页字段
|total|string|	记录总数
|prev|string|上一页 无上一页输出 -1
|next|string|下一页 无下一页输出 -1


###结果样例
---

    {
	"result": [{
		"cid": "1100000049165",
		"name": "考拉直播间",
		"img": "http://image.kaolafm.net/mz/images/201504/a88963e1-07c5-4526-99a2-fe7adabca92a/default.jpg",
		"description": "名人、红人、大咖，做客考拉直播间，谈论不一样的生活。",
		"type": "0",
		"categoryId": "121",
		"categoryName": "脱口秀"
	}],
	"requestId": "ffzex14030.11452135622206550"
}

###错误信息

请参考错误代码释义
