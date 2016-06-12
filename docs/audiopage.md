##获取指定期(碎片)所在专辑最新分页功能
===
###请求方式
---

**GET** `http://open.kaolafm.com/v1/audio/page?appid={appid}&sign={sign}&openid={openid}&audioId={audioId}&pageSize={pageSize}`

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
| audioId   | Long |   是   |碎片ID
| pageSize    | Integer |   是   |每页数



###返回参数
---

| 参数名称 | 类型    | 描述 
|:------- |:-------:|:------|
|id	 | long	 | 碎片ID
| name	| string	| 碎片名称
| num	| Integer	| 期次
| albumName | string	| 专辑名称

| 分页字段
| total	| string	| 记录总数
| totalPage | Integer|总页数
| prev	| string	| 上一页 无上一页输出 -1
| next	| string	| 下一页 无下一页输出 -1




###结果样例
-----

    {
	"result": {
		"total": "973",
		"next": "2",
		"prev": "-1",
		"totalPage": 49,
		"list": [{
			"aid": "1000002072012",
			"cover": "http://image.kaolafm.net/mz/images/201510/79de75a0-c9fc-4d90-968d-e44acf139a9e/default.jpg",
			"albumId": "1100000000078",
			"albumName": "二货一箩筐",
			"title": "教室放荤片",
			"playurl": "http://image.kaolafm.net/mz/mp3_32/201512/76a50790-f5d3-4ee5-8676-895aa8775ad9.mp3",
			"duration": "381010",
			"categoryId": "143",
			"clockId": "",
			"intercutTime": "",
			"hostList": [{
				"name": "王钢蛋",
				"description": "萝莉脸 冷面笑匠，猥琐的内心掩盖不了小清新的内心追求，总幻想着来一场说走就走的旅行，却常常千里送X，落个人财两空",
				"img": "http://image.kaolafm.net/mz/images/201309/01b160e4-30a8-474c-bec5-83649adb36a0/default.jpg"
			},
			{
				"name": "小毛驴",
				"description": "我就是集女汉子软妹子于一身的小毛驴~",
				"img": "http://image.kaolafm.net/mz/images/201411/766d2483-6a9a-44a7-b6b1-06234cdebe9b/default.jpg"
			}],
			"albumDescription": "",
			"description": "一个练了三年散打的小哥们看我长的人高马大的，非要和我练练。不到两分钟我就把他按到地上一顿狂揍。他站起伤感的说：老子练了三年的散打居然被你按在地上一顿打，真是白练了。 。。“哼，难道我练过9年的广播体操，我会告诉你！哼，有真功夫的人就是这么低调。”",
			"publishDate": "1450281600000",
			"md5": "2bb1cda6bab01e0b2e99dff37de912f9",
			"fileSize": "1524384",
			"rate": "32",
			"number": 975,
			"listenNum": 4795,
			"likeNum": 12,
			"commentNum": 0
		},
		{
			"aid": "1000002071958",
			"cover": "http://image.kaolafm.net/mz/images/201510/79de75a0-c9fc-4d90-968d-e44acf139a9e/default.jpg",
			"albumId": "1100000000078",
			"albumName": "二货一箩筐",
			"title": "重口味，请带纸！",
			"playurl": "http://image.kaolafm.net/mz/mp3_32/201512/eed05e9a-acb8-471b-97c7-12ba6d5da876.mp3",
			"duration": "484298",
			"categoryId": "143",
			"clockId": "",
			"intercutTime": "",
			"hostList": [{
				"name": "王钢蛋",
				"description": "萝莉脸 冷面笑匠，猥琐的内心掩盖不了小清新的内心追求，总幻想着来一场说走就走的旅行，却常常千里送X，落个人财两空",
				"img": "http://image.kaolafm.net/mz/images/201309/01b160e4-30a8-474c-bec5-83649adb36a0/default.jpg"
			},
			{
				"name": "小毛驴",
				"description": "我就是集女汉子软妹子于一身的小毛驴~",
				"img": "http://image.kaolafm.net/mz/images/201411/766d2483-6a9a-44a7-b6b1-06234cdebe9b/default.jpg"
			}],
			"albumDescription": "",
			"description": "话说一位领导到边防部队体验生活，问士兵性生活怎么解决，士兵指着外面的母骆驼：都靠它。领导摇头。一个月之后，领导实在受不了，心想：认了，把骆驼弄我帐篷来。士兵把骆驼牵来，惊讶的看领导费半天劲把骆驼办了。完事后，领导感慨：你们每次都这么费事么? 士兵摇头：我们平时都是骑它去镇上找姑娘！",
			"publishDate": "1450195200000",
			"md5": "4586e3a42698cef9cd32469921d45fa4",
			"fileSize": "1937520",
			"rate": "32",
			"number": 974,
			"listenNum": 19049,
			"likeNum": 87,
			"commentNum": 0
		},
		{
			"aid": "1000002071949",
			"cover": "http://image.kaolafm.net/mz/images/201510/79de75a0-c9fc-4d90-968d-e44acf139a9e/default.jpg",
			"albumId": "1100000000078",
			"albumName": "二货一箩筐",
			"title": "粉红色bra",
			"playurl": "http://image.kaolafm.net/mz/mp3_32/201512/2bfececd-5776-4cc2-9e4c-2cb4a72e8be6.mp3",
			"duration": "432810",
			"categoryId": "143",
			"clockId": "",
			"intercutTime": "",
			"hostList": [{
				"name": "王钢蛋",
				"description": "萝莉脸 冷面笑匠，猥琐的内心掩盖不了小清新的内心追求，总幻想着来一场说走就走的旅行，却常常千里送X，落个人财两空",
				"img": "http://image.kaolafm.net/mz/images/201309/01b160e4-30a8-474c-bec5-83649adb36a0/default.jpg"
			},
			{
				"name": "小毛驴",
				"description": "我就是集女汉子软妹子于一身的小毛驴~",
				"img": "http://image.kaolafm.net/mz/images/201411/766d2483-6a9a-44a7-b6b1-06234cdebe9b/default.jpg"
			}],
			"albumDescription": "",
			"description": "老板是个烟鬼，老板娘不让老板抽烟，老板怕他媳妇所以不敢明着抽，每次他抽烟都让我给他把风，今天像往长一样，老板娘回来的时候，我在办公室门外很大声的咳嗽两声。然后老板娘直冲我走来，啪，一巴掌说：我忍你很久了，你再调戏我个试试。",
			"publishDate": "1450108800000",
			"md5": "f865db8f0d141d0aaa27a3ac4d6fa4b0",
			"fileSize": "1731600",
			"rate": "32",
			"number": 973,
			"listenNum": 25348,
			"likeNum": 88,
			"commentNum": 0
		},
		{
			"aid": "1000002071931",
			"cover": "http://image.kaolafm.net/mz/images/201510/79de75a0-c9fc-4d90-968d-e44acf139a9e/default.jpg",
			"albumId": "1100000000078",
			"albumName": "二货一箩筐",
			"title": "玉米地里秘密",
			"playurl": "http://image.kaolafm.net/mz/mp3_32/201512/1628037a-33ec-488e-be27-0ea832ee80f3.mp3",
			"duration": "434456",
			"categoryId": "143",
			"clockId": "",
			"intercutTime": "",
			"hostList": [{
				"name": "王钢蛋",
				"description": "萝莉脸 冷面笑匠，猥琐的内心掩盖不了小清新的内心追求，总幻想着来一场说走就走的旅行，却常常千里送X，落个人财两空",
				"img": "http://image.kaolafm.net/mz/images/201309/01b160e4-30a8-474c-bec5-83649adb36a0/default.jpg"
			},
			{
				"name": "小毛驴",
				"description": "我就是集女汉子软妹子于一身的小毛驴~",
				"img": "http://image.kaolafm.net/mz/images/201411/766d2483-6a9a-44a7-b6b1-06234cdebe9b/default.jpg"
			}],
			"albumDescription": "",
			"description": "跟媳妇搞对象那会儿。有次带媳妇看完电影，骑自行车送她回家。经过她们村的一片玉米地时，她突然就从自行车上蹦了下来，把我也拽停，扯着我的衣服就往玉米地里钻。\r\n我受宠若惊，吓得小心脏扑通扑通跳……于是，在那个阳光明媚的晌午，我就这样被媳妇拉着，羞涩的第一次在地里见了她的父母，并且帮他们掰了一晌午的玉米棒子！\r\n",
			"publishDate": "1450022400000",
			"md5": "c0381d75bb04b14d46b5dfaddcd9df76",
			"fileSize": "1738224",
			"rate": "32",
			"number": 972,
			"listenNum": 31962,
			"likeNum": 115,
			"commentNum": 0
		},
		{
			"aid": "1000002062450",
			"cover": "http://image.kaolafm.net/mz/images/201510/79de75a0-c9fc-4d90-968d-e44acf139a9e/default.jpg",
			"albumId": "1100000000078",
			"albumName": "二货一箩筐",
			"title": "是不是真胸",
			"playurl": "http://image.kaolafm.net/mz/mp3_32/201512/ff70717c-4ee9-4675-b7b7-1b8dd102066d.mp3",
			"duration": "437199",
			"categoryId": "143",
			"clockId": "",
			"intercutTime": "",
			"hostList": [{
				"name": "王钢蛋",
				"description": "萝莉脸 冷面笑匠，猥琐的内心掩盖不了小清新的内心追求，总幻想着来一场说走就走的旅行，却常常千里送X，落个人财两空",
				"img": "http://image.kaolafm.net/mz/images/201309/01b160e4-30a8-474c-bec5-83649adb36a0/default.jpg"
			},
			{
				"name": "小毛驴",
				"description": "我就是集女汉子软妹子于一身的小毛驴~",
				"img": "http://image.kaolafm.net/mz/images/201411/766d2483-6a9a-44a7-b6b1-06234cdebe9b/default.jpg"
			}],
			"albumDescription": "",
			"description": "一女同事喝醉，我送她到家,正考虑要不要做点儿坏事儿,这时候出来俩小人，魔鬼说，你特么还想什么？上啊。天使说“你不能做龌蹉的事。”我正听他俩吵架，结果女同事一巴掌把天使拍死在墙上了…",
			"publishDate": "1449936000000",
			"md5": "a25acf98fcfcbff97ea07e5ddd8e5966",
			"fileSize": "1749168",
			"rate": "32",
			"number": 971,
			"listenNum": 38196,
			"likeNum": 133,
			"commentNum": 0
		},
		{
			"aid": "1000002071889",
			"cover": "http://image.kaolafm.net/mz/images/201510/79de75a0-c9fc-4d90-968d-e44acf139a9e/default.jpg",
			"albumId": "1100000000078",
			"albumName": "二货一箩筐",
			"title": "停电了，别摸我！-01",
			"playurl": "http://image.kaolafm.net/mz/mp3_32/201512/c9309ade-f36a-466c-8ebf-b77804697980.mp3",
			"duration": "1958675",
			"categoryId": "143",
			"clockId": "",
			"intercutTime": "",
			"hostList": [{
				"name": "王钢蛋",
				"description": "萝莉脸 冷面笑匠，猥琐的内心掩盖不了小清新的内心追求，总幻想着来一场说走就走的旅行，却常常千里送X，落个人财两空",
				"img": "http://image.kaolafm.net/mz/images/201309/01b160e4-30a8-474c-bec5-83649adb36a0/default.jpg"
			},
			{
				"name": "小毛驴",
				"description": "我就是集女汉子软妹子于一身的小毛驴~",
				"img": "http://image.kaolafm.net/mz/images/201411/766d2483-6a9a-44a7-b6b1-06234cdebe9b/default.jpg"
			}],
			"albumDescription": "",
			"description": "高三晚自习，化学老师在上面汫练习，我低下头玩手机.突然停电了，整个教室里同学的脸都亮了，我到现在还记得化学老师在手电筒下狰狞的脸啊!",
			"publishDate": "1449849600000",
			"md5": "d4a31c51ba9c6f0df420947640edaf01",
			"fileSize": "7835040",
			"rate": "32",
			"number": 970,
			"listenNum": 48396,
			"likeNum": 373,
			"commentNum": 0
		},
		{
			"aid": "1000002071878",
			"cover": "http://image.kaolafm.net/mz/images/201510/79de75a0-c9fc-4d90-968d-e44acf139a9e/default.jpg",
			"albumId": "1100000000078",
			"albumName": "二货一箩筐",
			"title": "停电了，别摸我！-02",
			"playurl": "http://image.kaolafm.net/mz/mp3_32/201512/890a2288-955c-49ef-af21-726835e22453.mp3",
			"duration": "1423034",
			"categoryId": "143",
			"clockId": "",
			"intercutTime": "",
			"hostList": [{
				"name": "王钢蛋",
				"description": "萝莉脸 冷面笑匠，猥琐的内心掩盖不了小清新的内心追求，总幻想着来一场说走就走的旅行，却常常千里送X，落个人财两空",
				"img": "http://image.kaolafm.net/mz/images/201309/01b160e4-30a8-474c-bec5-83649adb36a0/default.jpg"
			},
			{
				"name": "小毛驴",
				"description": "我就是集女汉子软妹子于一身的小毛驴~",
				"img": "http://image.kaolafm.net/mz/images/201411/766d2483-6a9a-44a7-b6b1-06234cdebe9b/default.jpg"
			}],
			"albumDescription": "",
			"description": "停电了,和单位的男神一起困在电梯里，本来应该装一下柔弱，但是因为上班快迟到了，于是就和男神两个人徒手把电梯搿开……从此男神这样介绍我的:这是我的患难好兄弟!",
			"publishDate": "1449849600000",
			"md5": "c158e97aabb4f9140bf882831901299f",
			"fileSize": "5692464",
			"rate": "32",
			"number": 969,
			"listenNum": 25708,
			"likeNum": 61,
			"commentNum": 0
		},
		{
			"aid": "1000002071844",
			"cover": "http://image.kaolafm.net/mz/images/201510/79de75a0-c9fc-4d90-968d-e44acf139a9e/default.jpg",
			"albumId": "1100000000078",
			"albumName": "二货一箩筐",
			"title": "停电了，别摸我！-03",
			"playurl": "http://image.kaolafm.net/mz/mp3_32/201512/30e0966c-0f82-4a8d-a3a1-2025f0cac631.mp3",
			"duration": "1060324",
			"categoryId": "143",
			"clockId": "",
			"intercutTime": "",
			"hostList": [{
				"name": "王钢蛋",
				"description": "萝莉脸 冷面笑匠，猥琐的内心掩盖不了小清新的内心追求，总幻想着来一场说走就走的旅行，却常常千里送X，落个人财两空",
				"img": "http://image.kaolafm.net/mz/images/201309/01b160e4-30a8-474c-bec5-83649adb36a0/default.jpg"
			},
			{
				"name": "小毛驴",
				"description": "我就是集女汉子软妹子于一身的小毛驴~",
				"img": "http://image.kaolafm.net/mz/images/201411/766d2483-6a9a-44a7-b6b1-06234cdebe9b/default.jpg"
			}],
			"albumDescription": "",
			"description": "高中毕业以后,我们班聚会，正吃着突然停电了。班长担心别人偷吃菜，就建议大家拍手唱歌。正在拍手唱歌唱到一半时电突然来了，大家一看，班长正在一手夹菜一手打自己耳光。",
			"publishDate": "1449849600000",
			"md5": "61c939ba1c44a5b2501b144f3cecff31",
			"fileSize": "4241664",
			"rate": "32",
			"number": 968,
			"listenNum": 22989,
			"likeNum": 38,
			"commentNum": 0
		},
		{
			"aid": "1000002062446",
			"cover": "http://image.kaolafm.net/mz/images/201510/79de75a0-c9fc-4d90-968d-e44acf139a9e/default.jpg",
			"albumId": "1100000000078",
			"albumName": "二货一箩筐",
			"title": "三里屯不眠夜",
			"playurl": "http://image.kaolafm.net/mz/mp3_32/201512/ca4ffa7b-84c7-4489-83ab-61b9b9f8cf3c.mp3",
			"duration": "436076",
			"categoryId": "143",
			"clockId": "",
			"intercutTime": "",
			"hostList": [{
				"name": "王钢蛋",
				"description": "萝莉脸 冷面笑匠，猥琐的内心掩盖不了小清新的内心追求，总幻想着来一场说走就走的旅行，却常常千里送X，落个人财两空",
				"img": "http://image.kaolafm.net/mz/images/201309/01b160e4-30a8-474c-bec5-83649adb36a0/default.jpg"
			},
			{
				"name": "小毛驴",
				"description": "我就是集女汉子软妹子于一身的小毛驴~",
				"img": "http://image.kaolafm.net/mz/images/201411/766d2483-6a9a-44a7-b6b1-06234cdebe9b/default.jpg"
			}],
			"albumDescription": "",
			"description": "小学时，有次数学考试，由于紧张，要交卷，发现没写名字，关键我竟然忘了自己叫什么……又不敢翻书，怕误以为作弊，正在我左右为难时，灵光一闪，我迅速的给了我同桌一耳光，只见他哭着对老师说：老师，王钢蛋打我。 终于我满意的写上了自己的名字。 至今我依然为我当初的机智感动。",
			"publishDate": "1449763200000",
			"md5": "c6fa551efd815d887c74dd423a8c1599",
			"fileSize": "1744704",
			"rate": "32",
			"number": 967,
			"listenNum": 30091,
			"likeNum": 127,
			"commentNum": 0
		},
		{
			"aid": "1000002062444",
			"cover": "http://image.kaolafm.net/mz/images/201510/79de75a0-c9fc-4d90-968d-e44acf139a9e/default.jpg",
			"albumId": "1100000000078",
			"albumName": "二货一箩筐",
			"title": "你是我的葫芦娃",
			"playurl": "http://image.kaolafm.net/mz/mp3_32/201512/d3d8ec33-a474-4893-9ad3-406c1c67f086.mp3",
			"duration": "440020",
			"categoryId": "143",
			"clockId": "",
			"intercutTime": "",
			"hostList": [{
				"name": "王钢蛋",
				"description": "萝莉脸 冷面笑匠，猥琐的内心掩盖不了小清新的内心追求，总幻想着来一场说走就走的旅行，却常常千里送X，落个人财两空",
				"img": "http://image.kaolafm.net/mz/images/201309/01b160e4-30a8-474c-bec5-83649adb36a0/default.jpg"
			},
			{
				"name": "小毛驴",
				"description": "我就是集女汉子软妹子于一身的小毛驴~",
				"img": "http://image.kaolafm.net/mz/images/201411/766d2483-6a9a-44a7-b6b1-06234cdebe9b/default.jpg"
			}],
			"albumDescription": "",
			"description": "公司的同事，孩子刚刚满月，一早上就挨个通知到下礼拜天去喝喜酒，完了我就听到坐我边上的大波嘟囔了句：“喝什么喜酒，孩子又不是我的！不去…！“ 这是我听到最牛逼的，不想随份子钱的理由！！",
			"publishDate": "1449676800000",
			"md5": "753feb65cba407b6257f824b733e5667",
			"fileSize": "1760400",
			"rate": "32",
			"number": 966,
			"listenNum": 41591,
			"likeNum": 203,
			"commentNum": 0
		},
		{
			"aid": "1000002062440",
			"cover": "http://image.kaolafm.net/mz/images/201510/79de75a0-c9fc-4d90-968d-e44acf139a9e/default.jpg",
			"albumId": "1100000000078",
			"albumName": "二货一箩筐",
			"title": "小姨子和小表妹",
			"playurl": "http://image.kaolafm.net/mz/mp3_32/201512/76c1efd9-b5db-448a-8b6a-ef14dafa2016.mp3",
			"duration": "443181",
			"categoryId": "143",
			"clockId": "",
			"intercutTime": "",
			"hostList": [{
				"name": "王钢蛋",
				"description": "萝莉脸 冷面笑匠，猥琐的内心掩盖不了小清新的内心追求，总幻想着来一场说走就走的旅行，却常常千里送X，落个人财两空",
				"img": "http://image.kaolafm.net/mz/images/201309/01b160e4-30a8-474c-bec5-83649adb36a0/default.jpg"
			},
			{
				"name": "小毛驴",
				"description": "我就是集女汉子软妹子于一身的小毛驴~",
				"img": "http://image.kaolafm.net/mz/images/201411/766d2483-6a9a-44a7-b6b1-06234cdebe9b/default.jpg"
			}],
			"albumDescription": "",
			"description": "昨晚和老婆啪啪啪后，用床头的纸巾擦了，太累直接睡，没有检查，丁丁上沾了纸巾，就直接睡着。第二天直接穿衣收拾上班，中午上厕所，同事大波在旁边瞄了一眼，说：你还挺自爱的，给丁丁做面膜啊。",
			"publishDate": "1449590400000",
			"md5": "e4f06ed399907a580ae0c43964e51435",
			"fileSize": "1773072",
			"rate": "32",
			"number": 965,
			"listenNum": 44941,
			"likeNum": 137,
			"commentNum": 0
		},
		{
			"aid": "1000002043424",
			"cover": "http://image.kaolafm.net/mz/images/201510/79de75a0-c9fc-4d90-968d-e44acf139a9e/default.jpg",
			"albumId": "1100000000078",
			"albumName": "二货一箩筐",
			"title": "贿赂体育老师",
			"playurl": "http://image.kaolafm.net/mz/mp3_32/201512/4e084e99-d2a8-4cc7-b002-abe6c1d2f062.mp3",
			"duration": "416719",
			"categoryId": "143",
			"clockId": "",
			"intercutTime": "",
			"hostList": [{
				"name": "王钢蛋",
				"description": "萝莉脸 冷面笑匠，猥琐的内心掩盖不了小清新的内心追求，总幻想着来一场说走就走的旅行，却常常千里送X，落个人财两空",
				"img": "http://image.kaolafm.net/mz/images/201309/01b160e4-30a8-474c-bec5-83649adb36a0/default.jpg"
			},
			{
				"name": "小毛驴",
				"description": "我就是集女汉子软妹子于一身的小毛驴~",
				"img": "http://image.kaolafm.net/mz/images/201411/766d2483-6a9a-44a7-b6b1-06234cdebe9b/default.jpg"
			}],
			"albumDescription": "",
			"description": "刚刚去上厕所,见垃圾桶旁边个大中华香烟盒子，默默捡了起来，掏出我的红双喜，塞进大中华空盒子！……上了厕所回来看见老板：捡起了我丢的空红双喜盒子，掏出他的大中华，抽出香烟、塞进空的红双喜盒子。",
			"publishDate": "1449504000000",
			"md5": "ef16d1d684d626ddcf72e5a2a34427cd",
			"fileSize": "1667232",
			"rate": "32",
			"number": 964,
			"listenNum": 49922,
			"likeNum": 133,
			"commentNum": 0
		},
		{
			"aid": "1000002040713",
			"cover": "http://image.kaolafm.net/mz/images/201510/79de75a0-c9fc-4d90-968d-e44acf139a9e/default.jpg",
			"albumId": "1100000000078",
			"albumName": "二货一箩筐",
			"title": "胸小的女生",
			"playurl": "http://image.kaolafm.net/mz/mp3_32/201511/1b1c86ff-cdc0-44b3-8eb1-126034f9e996.mp3",
			"duration": "437617",
			"categoryId": "143",
			"clockId": "",
			"intercutTime": "",
			"hostList": [{
				"name": "王钢蛋",
				"description": "萝莉脸 冷面笑匠，猥琐的内心掩盖不了小清新的内心追求，总幻想着来一场说走就走的旅行，却常常千里送X，落个人财两空",
				"img": "http://image.kaolafm.net/mz/images/201309/01b160e4-30a8-474c-bec5-83649adb36a0/default.jpg"
			},
			{
				"name": "小毛驴",
				"description": "我就是集女汉子软妹子于一身的小毛驴~",
				"img": "http://image.kaolafm.net/mz/images/201411/766d2483-6a9a-44a7-b6b1-06234cdebe9b/default.jpg"
			}],
			"albumDescription": "",
			"description": "告诉大家一个好消息，如果想要抢手机不用在大街上抢，去公共厕所抢好，因为很多人都是一边拉屎一边玩手机的，这样去抢的话成功率百分百，不用谢我，一般人我不告诉他的。不说了，擦腚追手机去了！",
			"publishDate": "1449417600000",
			"md5": "baada061074995b95061bf5f039e33b7",
			"fileSize": "1750896",
			"rate": "32",
			"number": 963,
			"listenNum": 53491,
			"likeNum": 144,
			"commentNum": 0
		},
		{
			"aid": "1000002043419",
			"cover": "http://image.kaolafm.net/mz/images/201510/79de75a0-c9fc-4d90-968d-e44acf139a9e/default.jpg",
			"albumId": "1100000000078",
			"albumName": "二货一箩筐",
			"title": "朋友圈卖内衣",
			"playurl": "http://image.kaolafm.net/mz/mp3_32/201512/62980e79-1d4d-4cfd-8308-c2aa485533a9.mp3",
			"duration": "471393",
			"categoryId": "143",
			"clockId": "",
			"intercutTime": "",
			"hostList": [{
				"name": "王钢蛋",
				"description": "萝莉脸 冷面笑匠，猥琐的内心掩盖不了小清新的内心追求，总幻想着来一场说走就走的旅行，却常常千里送X，落个人财两空",
				"img": "http://image.kaolafm.net/mz/images/201309/01b160e4-30a8-474c-bec5-83649adb36a0/default.jpg"
			},
			{
				"name": "小毛驴",
				"description": "我就是集女汉子软妹子于一身的小毛驴~",
				"img": "http://image.kaolafm.net/mz/images/201411/766d2483-6a9a-44a7-b6b1-06234cdebe9b/default.jpg"
			}],
			"albumDescription": "",
			"description": "上大学的时候,一大冷天铁锤跟我提了个很荒唐的请求，这不要脸的竟然说要跟我换女朋友啪啪啪，我反手就是一巴掌：“你特么是不是岛国片看多了？”劳资果断拒绝！特么你那林志玲破成那样，十几个补丁，想跟我这上星期刚到货的冰冰换？",
			"publishDate": "1449331200000",
			"md5": "cc355c1e3266bf1dbdf4de46bde1581f",
			"fileSize": "1885968",
			"rate": "32",
			"number": 962,
			"listenNum": 56927,
			"likeNum": 164,
			"commentNum": 0
		},
		{
			"aid": "1000002051134",
			"cover": "http://image.kaolafm.net/mz/images/201510/79de75a0-c9fc-4d90-968d-e44acf139a9e/default.jpg",
			"albumId": "1100000000078",
			"albumName": "二货一箩筐",
			"title": "大姐，打打打个劫！-01",
			"playurl": "http://image.kaolafm.net/mz/mp3_32/201512/bfd2608e-f8f8-4a2d-9d4a-bdb709705f3f.mp3",
			"duration": "1324579",
			"categoryId": "143",
			"clockId": "",
			"intercutTime": "",
			"hostList": [{
				"name": "王钢蛋",
				"description": "萝莉脸 冷面笑匠，猥琐的内心掩盖不了小清新的内心追求，总幻想着来一场说走就走的旅行，却常常千里送X，落个人财两空",
				"img": "http://image.kaolafm.net/mz/images/201309/01b160e4-30a8-474c-bec5-83649adb36a0/default.jpg"
			},
			{
				"name": "小毛驴",
				"description": "我就是集女汉子软妹子于一身的小毛驴~",
				"img": "http://image.kaolafm.net/mz/images/201411/766d2483-6a9a-44a7-b6b1-06234cdebe9b/default.jpg"
			}],
			"albumDescription": "",
			"description": "无父无母的少年被杀手集团收养，第一次看杀手拿刀给人分尸，少年问他：“怎么才能变得和你这样冷血麻木呢。”杀手冷哼一声：“你剁你也麻。”   ",
			"publishDate": "1449244800000",
			"md5": "ce67c691433ae853779287f1b1d5492d",
			"fileSize": "5298624",
			"rate": "32",
			"number": 961,
			"listenNum": 58001,
			"likeNum": 336,
			"commentNum": 0
		},
		{
			"aid": "1000002051131",
			"cover": "http://image.kaolafm.net/mz/images/201510/79de75a0-c9fc-4d90-968d-e44acf139a9e/default.jpg",
			"albumId": "1100000000078",
			"albumName": "二货一箩筐",
			"title": "大姐，打打打个劫！-02",
			"playurl": "http://image.kaolafm.net/mz/mp3_32/201512/dd36b2f8-2bf3-4f56-b526-20242ad758c0.mp3",
			"duration": "1677676",
			"categoryId": "143",
			"clockId": "",
			"intercutTime": "",
			"hostList": [{
				"name": "王钢蛋",
				"description": "萝莉脸 冷面笑匠，猥琐的内心掩盖不了小清新的内心追求，总幻想着来一场说走就走的旅行，却常常千里送X，落个人财两空",
				"img": "http://image.kaolafm.net/mz/images/201309/01b160e4-30a8-474c-bec5-83649adb36a0/default.jpg"
			},
			{
				"name": "小毛驴",
				"description": "我就是集女汉子软妹子于一身的小毛驴~",
				"img": "http://image.kaolafm.net/mz/images/201411/766d2483-6a9a-44a7-b6b1-06234cdebe9b/default.jpg"
			}],
			"albumDescription": "",
			"description": "最近有很多人都在黑气功，我觉得你们懂个屁，气功曾经救过我一命。在我16岁那年，曾被一群小流氓打劫，当时我就使用了龟派气功对付他们。带头的那个混混临走前对我说：要不是看你是个傻B，我早TM揍死你了。",
			"publishDate": "1449244800000",
			"md5": "feb2c35f470aefa84174cf8cd9c34833",
			"fileSize": "6711120",
			"rate": "32",
			"number": 960,
			"listenNum": 40420,
			"likeNum": 98,
			"commentNum": 0
		},
		{
			"aid": "1000002051123",
			"cover": "http://image.kaolafm.net/mz/images/201510/79de75a0-c9fc-4d90-968d-e44acf139a9e/default.jpg",
			"albumId": "1100000000078",
			"albumName": "二货一箩筐",
			"title": "大姐，打打打个劫！-03",
			"playurl": "http://image.kaolafm.net/mz/mp3_32/201512/08aeb22c-1209-4a80-9bf9-00414445ca1e.mp3",
			"duration": "1109382",
			"categoryId": "143",
			"clockId": "",
			"intercutTime": "",
			"hostList": [{
				"name": "王钢蛋",
				"description": "萝莉脸 冷面笑匠，猥琐的内心掩盖不了小清新的内心追求，总幻想着来一场说走就走的旅行，却常常千里送X，落个人财两空",
				"img": "http://image.kaolafm.net/mz/images/201309/01b160e4-30a8-474c-bec5-83649adb36a0/default.jpg"
			},
			{
				"name": "小毛驴",
				"description": "我就是集女汉子软妹子于一身的小毛驴~",
				"img": "http://image.kaolafm.net/mz/images/201411/766d2483-6a9a-44a7-b6b1-06234cdebe9b/default.jpg"
			}],
			"albumDescription": "",
			"description": "一贯淘气、不交家庭作业的王钢蛋上学来晚了。老师：“王钢蛋，你咋又来迟到了？”\r\n王钢蛋故作张口气喘：“老师，不好了，来学校的路上，我被人打劫了？”老师：“天哪，那贼伤害你哪里没有？” 王钢蛋：“到没打我，嫌我只有2元钱太少，没要。”老师：“那他要你啥了？”王钢蛋：“把我家庭作业本给抢去了。”\r\n",
			"publishDate": "1449244800000",
			"md5": "3b61d10853fc1fcd530dd8e9d0c4c3a9",
			"fileSize": "4437936",
			"rate": "32",
			"number": 959,
			"listenNum": 31765,
			"likeNum": 43,
			"commentNum": 0
		},
		{
			"aid": "1000002043422",
			"cover": "http://image.kaolafm.net/mz/images/201510/79de75a0-c9fc-4d90-968d-e44acf139a9e/default.jpg",
			"albumId": "1100000000078",
			"albumName": "二货一箩筐",
			"title": "公车里的变态",
			"playurl": "http://image.kaolafm.net/mz/mp3_32/201512/8881ba1c-5d8e-4982-bf00-e2bd8ab4f30e.mp3",
			"duration": "474868",
			"categoryId": "143",
			"clockId": "",
			"intercutTime": "",
			"hostList": [{
				"name": "王钢蛋",
				"description": "萝莉脸 冷面笑匠，猥琐的内心掩盖不了小清新的内心追求，总幻想着来一场说走就走的旅行，却常常千里送X，落个人财两空",
				"img": "http://image.kaolafm.net/mz/images/201309/01b160e4-30a8-474c-bec5-83649adb36a0/default.jpg"
			},
			{
				"name": "小毛驴",
				"description": "我就是集女汉子软妹子于一身的小毛驴~",
				"img": "http://image.kaolafm.net/mz/images/201411/766d2483-6a9a-44a7-b6b1-06234cdebe9b/default.jpg"
			}],
			"albumDescription": "",
			"description": "网聊了一美女，经常说一些暧昧的话，终于有一天美女忍不住寂寞，约我开房。我火烧火了的打个车到酒店，一进房门愣了…… 美女挑眉：“你可真对的起你老婆啊。” 我膝盖一软就跪下了：“丈母娘我错了！",
			"publishDate": "1449158400000",
			"md5": "8c37f355ec0effa8073daefe16b7dcb1",
			"fileSize": "1899792",
			"rate": "32",
			"number": 958,
			"listenNum": 41807,
			"likeNum": 156,
			"commentNum": 0
		},
		{
			"aid": "1000002040712",
			"cover": "http://image.kaolafm.net/mz/images/201510/79de75a0-c9fc-4d90-968d-e44acf139a9e/default.jpg",
			"albumId": "1100000000078",
			"albumName": "二货一箩筐",
			"title": "心痛的赶脚",
			"playurl": "http://image.kaolafm.net/mz/mp3_32/201511/c8ecea71-51d9-476b-93de-504d8f25dce5.mp3",
			"duration": "459037",
			"categoryId": "143",
			"clockId": "",
			"intercutTime": "",
			"hostList": [{
				"name": "王钢蛋",
				"description": "萝莉脸 冷面笑匠，猥琐的内心掩盖不了小清新的内心追求，总幻想着来一场说走就走的旅行，却常常千里送X，落个人财两空",
				"img": "http://image.kaolafm.net/mz/images/201309/01b160e4-30a8-474c-bec5-83649adb36a0/default.jpg"
			},
			{
				"name": "小毛驴",
				"description": "我就是集女汉子软妹子于一身的小毛驴~",
				"img": "http://image.kaolafm.net/mz/images/201411/766d2483-6a9a-44a7-b6b1-06234cdebe9b/default.jpg"
			}],
			"albumDescription": "",
			"description": "毛驴我在办公室养了半个月的小鱼死了，我伤心极了，心想一定要给它办个隆重的葬礼，埋土里吧，怕猫挖；水葬吧，怕沉下去被下水道的老鼠祸害，再三考虑后决定给它办个火葬，于是找钢蛋借来打火机，谁知道特么的越烤越香…………不说了，我在忏悔呢。",
			"publishDate": "1449072000000",
			"md5": "e56b1bedc2422f52ac12686ec7739a41",
			"fileSize": "1836576",
			"rate": "32",
			"number": 957,
			"listenNum": 47400,
			"likeNum": 150,
			"commentNum": 0
		},
		{
			"aid": "1000002040710",
			"cover": "http://image.kaolafm.net/mz/images/201510/79de75a0-c9fc-4d90-968d-e44acf139a9e/default.jpg",
			"albumId": "1100000000078",
			"albumName": "二货一箩筐",
			"title": "可爱的日本妹子",
			"playurl": "http://image.kaolafm.net/mz/mp3_32/201511/70ba024b-1e62-4ebe-ab5a-4e19949a4622.mp3",
			"duration": "446943",
			"categoryId": "143",
			"clockId": "",
			"intercutTime": "",
			"hostList": [{
				"name": "王钢蛋",
				"description": "萝莉脸 冷面笑匠，猥琐的内心掩盖不了小清新的内心追求，总幻想着来一场说走就走的旅行，却常常千里送X，落个人财两空",
				"img": "http://image.kaolafm.net/mz/images/201309/01b160e4-30a8-474c-bec5-83649adb36a0/default.jpg"
			},
			{
				"name": "小毛驴",
				"description": "我就是集女汉子软妹子于一身的小毛驴~",
				"img": "http://image.kaolafm.net/mz/images/201411/766d2483-6a9a-44a7-b6b1-06234cdebe9b/default.jpg"
			}],
			"albumDescription": "",
			"description": "哥们铁锤对公司的经理很不满，想辞职走人了，临走想写封气死他的辞职信，于是发短信求助我，钢蛋我在职场混迹多年，回复他的短信只有短短9个字：经理你好，你老婆好紧。",
			"publishDate": "1448985600000",
			"md5": "ea94e403adf0258b9886fc7a0b76444c",
			"fileSize": "1788192",
			"rate": "32",
			"number": 956,
			"listenNum": 51789,
			"likeNum": 196,
			"commentNum": 0
		}]
	},
	"requestId": "tgdbv86810.11450320017006151"
}

###错误信息

请参考错误代码释义
