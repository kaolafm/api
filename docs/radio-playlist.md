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
| number	| string	| 期数
| publishDate | String  | 上线日期（毫秒）
| md5   | String  | 文件md5
| rate  | String  | 当前码率
| fileSize | String | 文件大小(字节）



###结果样例
---

    {

    "result": [
        {
            "aid": "1000000758962",
            "cover": null,
            "albumId": "1100000037152",
            "albumName": "SW-休闲FM-Tag-02",
            "title": "SW-休闲FM-Tag-02",
            "playurl": "http://image.kaolafm.net/mz/mp3_64/201411/2f4b3e7f-10c0-4aec-8be1-6ceb61c99805.mp3?appid=fiaju0644&deviceid=100000029020744&audioid=1000000758962",
            "duration": null,
            "categoryId": "131",
            "clockId": "",
            "intercutTime": "",
            "hostList": [ ],
            "albumDescription": "",
            "description": "",
            "publishDate": "1415257770000",
            "md5": "",
            "rate": "64",
            "number": 1,
            "fileSzie": ""
        },
        {
            "aid": "1000000002083",
            "cover": "http://image.kaolafm.net/mz/images/201501/a76e0100-1da2-44aa-aebe-095688b88336/default.jpg",
            "albumId": "1100000003620",
            "albumName": "你怎么舍得我难过",
            "title": "你怎么舍得我难过",
            "playurl": "http://image.kaolafm.net/mz/mp3_64/201402/ef60c2c3-2ed0-4321-84c4-0296cb52a2ac.mp3?appid=fiaju0644&deviceid=100000029020744&audioid=1000000002083",
            "duration": null,
            "categoryId": "129",
            "clockId": "",
            "intercutTime": "",
            "hostList": [
                {
                    "name": "黄小琥",
                    "description": "黄小琥1963年6月21日出生于台湾。\r\n1989年，黄小琥发行单曲《你是我最爱》，正式出道。1990年发行首张专辑《不只是朋友》，获得第二届金曲奖“最佳新人奖”以及“最佳录音奖”。1993年发行专辑《放纵玫瑰》。1994年发行专辑《飞越彩虹》，《我心孤独》。1996年发行专辑《午夜的单人床》。2001年发行个人创作专辑《她的歌》。\r\n2007年，担任超级星光大道客座评审 。2009年，发行的专辑《简单/不简单》在台湾地区销售量突破5万张。2010年，黄小琥凭借《没那么简单》走红，位居台湾2010年“10大KTV热门点播歌曲”第一位。",
                    "img": "http://image.kaolafm.net/mz/images/201410/a8ca8db0-4fc3-4073-a0f5-621e29ea996f/default.jpg"
                }
            ],
            "albumDescription": "",
            "description": "对你的思念是一天又一天\r\n孤单的我还是没有改变\r\n美丽的梦何时才能出现\r\n亲爱的你好想再见你一面\r\n\r\n秋天的风一阵阵的吹过\r\n想起了去年的这个时候\r\n你的心到底在想些什么\r\n为什么留下这个结局\r\n让我承受\r\n\r\n最爱你的人是我\r\n你怎么舍得我难过\r\n在我最需要你的时候\r\n没有说一句话就走\r\n最爱你的人是我\r\n你怎么舍得我难过\r\n对你付出了这么多\r\n你却没有感动过\r\n\r\n秋天的风一阵阵的吹过\r\n想起了去年的这个时候\r\n你的心到底在想些什么\r\n为什么留下这个结局\r\n让我承受\r\n\r\n最爱你的人是我\r\n你怎么舍得我难过\r\n在我最需要你的时候\r\n没有说一句话就走\r\n最爱你的人是我\r\n你怎么舍得我难过\r\n对你付出了这么多\r\n你却没有感动过\r\n\r\n最爱你的人是我\r\n你怎么舍得我难过\r\n在我最需要你的时候\r\n没有说一句话就走\r\n最爱你的人是我\r\n你怎么舍得我难过\r\n对你付出了这么多\r\n你却没有感动过 ",
            "publishDate": "1392026413000",
            "md5": "",
            "rate": "64",
            "number": 1,
            "fileSzie": ""
        },
        {
            "aid": "1000000001692",
            "cover": "http://image.kaolafm.net/mz/images/201501/c5cdf1ce-78af-4418-9b5d-8ebd3e66775f/default.jpg",
            "albumId": "1100000003502",
            "albumName": "伤心对我来说",
            "title": "伤心对我来说",
            "playurl": "http://image.kaolafm.net/mz/mp3_64/201401/eb0a9e51-1cbe-463e-8b42-9ec6b85df50a.mp3?appid=fiaju0644&deviceid=100000029020744&audioid=1000000001692",
            "duration": null,
            "categoryId": "129",
            "clockId": "",
            "intercutTime": "",
            "hostList": [
                {
                    "name": "高明骏",
                    "description": "高明骏台湾著名歌手，先后发行十张个人专辑（台湾九张，大陆一张）。1988年首张《年轻的喝彩》在台湾一炮而红，后陆续推出九张个人专辑。一首《我悄悄地蒙上你的眼睛》更在大陆广为传唱。2000年定居北京，2006年推出第十张个人专辑《现在回家》，07年单曲《在水一方 爱的箴言》，08年《绽放》，09年《男人四十》，11年《时间在路上》，12年《春生的爱情》。一直不断在做音乐的他依旧保持着那性感苍凉、狂野奔放的嗓音。热爱生活的他，喜欢自己研究美食，喜欢携家人自驾旅行。音乐、家庭、美食、旅行已经构成了他生活的重要四个组成部分。",
                    "img": "http://image.kaolafm.net/mz/images/201410/f0edb3f7-669e-402a-a5f1-e35440c7e674/default.jpg"
                }
            ],
            "albumDescription": "",
            "description": "爱 情 对我来说 \r\n它是让我宿醉的纯酒\r\n\r\n可是爱情 对你来说 \r\n只是续一杯 免费 的咖啡\r\n\r\nOH 伤 害对我来说\r\n怕是不可避免的结果\r\n\r\n可是伤害 对你来说\r\n只是又一 次 不经意的过错\r\n\r\nHONEY H O N E Y\r\n我没有 错\r\nHONEY H O N E Y\r\n我该如 何\r\n\r\n对你付出 已太多\r\n对你要求 没有过\r\nHONEY H O N E Y\r\n我该怎么做\r\n\r\nHO NEY 有个 女 孩\r\n她也曾经对我 这么说\r\n不 知 分开 对她来说\r\n伤心是否 和我现在 一样多\r\n\r\nOH HONEY 在你心中\r\n我是否只是其中 的一个\r\n可是 伤 心 对我来说\r\n却是第一次 也是最后 一次的结果\r\n\r\nHONEY H O N E Y\r\n我没有 错 \r\nHONEY H O N E Y\r\n我该如 何 \r\n\r\n对你付出 已太多 \r\n对你要求 没有过\r\nHONEY H O N E Y\r\n我该怎么做 \r\n\r\nHONEY H O N E Y\r\n我没有 错哦 \r\nHONEY H O N E Y\r\n我该如 何\r\n\r\n对你付出 已太多 \r\n对你要求 没有过\r\nHONEY H O N E Y\r\n我该怎么做 ",
            "publishDate": "1390728621000",
            "md5": "",
            "rate": "64",
            "number": 1,
            "fileSzie": ""
        },
        {
            "aid": "1000000019653",
            "cover": "http://image.kaolafm.net/mz/images/201404/3705b65e-3ed8-4631-83e5-cda825ceef69/default.jpg",
            "albumId": "1100000006744",
            "albumName": "Smoke Gets In Your Eyes",
            "title": "Smoke Gets In Your Eyes",
            "playurl": "http://image.kaolafm.net/mz/mp3_64/201404/f9422dbf-ac04-4f8e-bb04-664422403cc0.mp3?appid=fiaju0644&deviceid=100000029020744&audioid=1000000019653",
            "duration": null,
            "categoryId": "129",
            "clockId": "",
            "intercutTime": "",
            "hostList": [
                {
                    "name": "The Platters",
                    "description": "THE PLATTERS是流行音乐史上第一支在热门流行榜上拥有冠军歌曲的黑人合唱团体。THE PLATTERS发行的第一首ONLY YOU，原本是一首布鲁斯风格的歌曲，经过他们以流行乐的方式演唱，从而成为黑人歌星的第一首全球畅销金牌榜。\r\n被誉为美国国宝级组合的五黑宝（The Platters）是50年代最顶尖的美声团体之一，亦是当时最受欢迎的黑人团体。由东尼威廉斯、大卫林奇、赫伯瑞德、保罗罗宾与罗拉泰勒组成，在摇滚乐盛行之前他们以流行抒情歌曲成功虏获乐迷的心，干净、完美无懈可击的优美和声，让人为之着迷。",
                    "img": "http://image.kaolafm.net/mz/images/201410/b93641e9-1575-4975-9392-8e1e7e98d56b/default.jpg"
                }
            ],
            "albumDescription": "",
            "description": "They asked me how I knew my true love was true. Oh,\r\nI of course replied\r\nsomething here inside cannot be denied.\r\nThey said someday youll find all who love are blind.\r\nOh,When your hearts on fire,\r\nyou must realize smoke gets in your eyes\r\nSo I chaffed them\r\nand I gaily laughed to think they could doubt my love.\r\nYet today my love has flown away, I am without my love.\r\nNow laughing friends deride tears I cannot hide. Oh,\r\nSo I smile and say\r\nwhen a lovely flame dies, smoke gets in your eyes!\r\nSmoke gets in your eyes\r\nSmoke gets in your eyes ",
            "publishDate": "1396404740000",
            "md5": "",
            "rate": "64",
            "number": 1,
            "fileSzie": ""
        },
        {
            "aid": "1000000017851",
            "cover": "http://image.kaolafm.net/mz/images/201404/ec360c08-d709-42ea-bfe6-d39e8c3a8d86/default.jpg",
            "albumId": "1100000006479",
            "albumName": "晚安",
            "title": "晚安",
            "playurl": "http://image.kaolafm.net/mz/mp3_64/201403/0875d88d-bc3c-491f-80be-5d3aea82aa21.mp3?appid=fiaju0644&deviceid=100000029020744&audioid=1000000017851",
            "duration": null,
            "categoryId": "129",
            "clockId": "",
            "intercutTime": "",
            "hostList": [
                {
                    "name": "林宥嘉",
                    "description": "林宥嘉，1987年7月1日出生于中国台湾屏东。\r\n2007年7月以大学生的身份，夺得台湾中视主办的歌唱选秀节目《超级星光大道》第一季冠军 ，并获华研音乐签约成为专属歌手 。演唱歌曲有《你把我灌醉》、《开到荼靡》、《我爱的人》和《你是我的眼》等。\r\n2010年10月18日获第十届CCTV-MTV音乐盛典港澳台地区年度最受欢迎潜力歌手奖 。代表作包括《说谎》、《神秘嘉宾》、《伯乐》、《我总是一个人在练习一个人》、《诱》等。",
                    "img": "http://image.kaolafm.net/mz/images/201410/c621101b-4967-4f36-807b-edf56db93379/default.jpg"
                }
            ],
            "albumDescription": "",
            "description": "天 空白着夜晚\r\n城市一片灯火扰乱\r\n风 吹过看不见的天堂\r\n是谁还在忙碌地追赶\r\n\r\n晚安 让记忆松绑\r\n忘掉所有痛苦悲伤\r\n让 所有听不见的呐喊\r\n随着黑夜一起埋葬\r\n\r\n月 亮在你心坎\r\n可曾把你的梦点燃\r\n心 疼你每一步的成长\r\n擦干眼泪变得更勇敢\r\n\r\n晚安 卸下了翅膀\r\n轻轻打开梦里的窗\r\n路 尽管依然会有阻挡\r\n让我陪你一起飞翔\r\n\r\n梦 想去的地方\r\n因为不变所以简单\r\n爱 如果早已经被遗忘\r\n我的歌声不会有伤感\r\n\r\n晚安 静静地安躺\r\n躺在可以放心的床\r\n夜 因为有了梦才宽敞\r\n因为有你所以温暖 ",
            "publishDate": "1395978383000",
            "md5": "",
            "rate": "64",
            "number": 1,
            "fileSzie": ""
        },
        {
            "aid": "1000000175600",
            "cover": "http://image.kaolafm.net/mz/images/201406/08864468-6f17-4dd6-8e9c-a99249f446a1/default.jpg",
            "albumId": "1100000011957",
            "albumName": "考拉FM-SW08",
            "title": "考拉FM-SW08",
            "playurl": "http://image.kaolafm.net/mz/mp3_64/201404/43b1835c-50ff-46c2-bf90-a9e4da8ca4e6.mp3?appid=fiaju0644&deviceid=100000029020744&audioid=1000000175600",
            "duration": null,
            "categoryId": "131",
            "clockId": "",
            "intercutTime": "",
            "hostList": [ ],
            "albumDescription": "",
            "description": "",
            "publishDate": "1411038121000",
            "md5": "",
            "rate": "64",
            "number": 1,
            "fileSzie": ""
        },
        {
            "aid": "1000000019302",
            "cover": "http://image.kaolafm.net/mz/images/201404/b12744e2-dc08-43ae-902a-8c0a927db85c/default.jpg",
            "albumId": "1100000006807",
            "albumName": "画心",
            "title": "画心",
            "playurl": "http://image.kaolafm.net/mz/mp3_64/201404/7a3041aa-dd89-49df-b755-71b811842086.mp3?appid=fiaju0644&deviceid=100000029020744&audioid=1000000019302",
            "duration": null,
            "categoryId": "129",
            "clockId": "",
            "intercutTime": "",
            "hostList": [
                {
                    "name": "张靓颖",
                    "description": "张靓颖（Jane Zhang），1984年10月11日生于四川成都，中国流行女歌手，毕业于四川大学外国语学院。2005年参加湖南卫视超级女声比赛荣获季军，赛后签约华友世纪和华谊兄弟，开始歌手生涯，7月发布个人首支单曲 《open up your dream 》。\r\n2006年10月发行第一张专辑《The One》，2007年9月1日，张靓颖凭借《我用所有报答爱》奖获香港电影金紫荆奖最佳电影歌曲。2008年，张靓颖首度与台湾地区组合三角cool合作演唱《功夫之王》片尾曲《Heroes》并演唱电影《画皮》主题曲《画心》，凭借《画心》获得香港电影金像奖最佳原创电影歌曲奖。",
                    "img": "http://image.kaolafm.net/mz/images/201412/f1947e73-1b35-4247-9817-f706230f9c09/default.jpg"
                }
            ],
            "albumDescription": "",
            "description": "啦啦啦 啦啦啦....... \r\n看不穿 是你失落的魂魄 \r\n猜不透 是你瞳孔的颜色 \r\n一阵风 一场梦 \r\n爱如生命般莫测 \r\n你的心 到底被什么蛊惑 \r\n你的轮廓在黑夜之中淹没 \r\n看桃花 开出怎样的结果 \r\n看着你抱着我 目光似月色寂寞 \r\n就让你 在别人怀里快乐 \r\n爱着你 像心跳难触摸 \r\n画着你 画不出你的骨骼 \r\n记着你的脸色 是我等你的执着 \r\n你是我 一首唱不完的歌 \r\n看不穿 是你失落的魂魄 \r\n猜不透 是你瞳孔的颜色 \r\n一阵风 一场梦 \r\n爱是生命的莫测 \r\n你的心到底被什么蛊惑 \r\n你的轮廓在黑夜之中淹没 \r\n看桃花开出怎样的结果 \r\n看着你抱着我 目光比月色寂寞 \r\n就让你 在别人怀里快乐 \r\n爱着你 像心跳难触摸 \r\n画着你 画不出你的骨骼 \r\n记着你的脸色 是我等你的执着 \r\n你是我 一首唱不完的歌 \r\n你的轮廓在黑夜之中淹没 \r\n看桃花开出怎样的结果 \r\n看着你抱着我 目光比月色寂寞 \r\n就让你 在别人怀里快乐 \r\n爱着你 像心跳难触摸 \r\n画着你 画不出你的骨骼 \r\n记着你的脸色 是我等你的执着 \r\n我的心 只愿为你而割舍 ",
            "publishDate": "1396516081000",
            "md5": "",
            "rate": "64",
            "number": 1,
            "fileSzie": ""
        },
        {
            "aid": "1000000019609",
            "cover": "http://image.kaolafm.net/mz/images/201404/a92f2ecf-676a-4587-9c43-86aa93d99aae/default.jpg",
            "albumId": "1100000006845",
            "albumName": "请你给我好一点的情敌",
            "title": "请你给我好一点的情敌",
            "playurl": "http://image.kaolafm.net/mz/mp3_64/201404/dca32cda-44b0-4bdd-8820-85e1a0af65a7.mp3?appid=fiaju0644&deviceid=100000029020744&audioid=1000000019609",
            "duration": null,
            "categoryId": "129",
            "clockId": "",
            "intercutTime": "",
            "hostList": [
                {
                    "name": "田馥甄",
                    "description": "田馥甄（Hebe），1983年3月30日出生于台湾省新竹县，华语女子演唱团体S.H.E的成员之一。\r\n2000年，田馥甄参加”宇宙2000实力美少女选拔大赛“获得殿军，赛后与参赛成员任家萱、陈嘉桦共同签入华研国际音乐，组成S.H.E组合，进入演艺圈。2010年以其本名发布首张个人专辑《To Hebe》；同年10月举办《Love!田馥甄To Hebe》巡回音乐会。2011年9月发行第二张个人专辑《My Love》，入围第23届金曲奖最佳国语专辑及最佳国语女歌手等奖项。2013年11月发行第三张个人专辑《渺小》，入围第25届金曲奖最佳专辑包装与最佳音乐录像带奖。",
                    "img": "http://image.kaolafm.net/mz/images/201410/ad750b0a-6276-4b98-89dd-5fe80562617a/default.jpg"
                }
            ],
            "albumDescription": "",
            "description": "这已经不是我第一次听到她的名字\r\n你是我们共同爱上的浪子\r\n其实我并不真的在乎\r\n与别人一起占有你\r\n我并不真的介意\r\n你的吻\r\n也盖着别人的印记\r\n\r\n如果这是你不能逃避的宿命\r\n就请你给我好一点的情敌\r\n至少让我拥有竞争的乐趣\r\n至少让我相信\r\n被遗弃\r\n有被遗弃的道理\r\n\r\n这已经不是我第一次听到她的故事\r\n你是我们共同爱上的主题\r\n其实我并不真的难过\r\n与他人一起分享所有\r\n我并不真的害怕\r\n你的爱\r\n左顾右盼牵牵挂挂\r\n\r\n如果这是我不能躲闪的结局\r\n我只要求给我好一点的情敌\r\n至少让我拥有完美的嫉妒\r\n至少让我感觉\r\n有另一人\r\n足以匹配我的孤独",
            "publishDate": "1397009369000",
            "md5": "",
            "rate": "64",
            "number": 1,
            "fileSzie": ""
        },
        {
            "aid": "1000001729025",
            "cover": "http://image.kaolafm.net/mz/images/201507/c0897454-38fa-4bbb-9175-0e723dd577ce/default.jpg",
            "albumId": "1100000063810",
            "albumName": "泪滴",
            "title": "泪滴",
            "playurl": "http://image.kaolafm.net/mz/mp3_64/201507/418e18d4-3d1d-4fd5-b6b4-b18d6b95310d.mp3?appid=fiaju0644&deviceid=100000029020744&audioid=1000001729025",
            "duration": null,
            "categoryId": "129",
            "clockId": "",
            "intercutTime": "",
            "hostList": [
                {
                    "name": "张清芳",
                    "description": "张清芳：（1966年8月31日－）英文名字Stella，金曲奖与金鼎奖“镀双金”华语世界天后级女歌手、电视与广播节目主持人，也曾尝试戏剧演出。张清芳1980年代即以学生歌手身份走红登峰，艺界持续力道惊人。二十年来，一直不靠绯闻炒作知名度，她令有人难望其项背的成绩，是华语流行音乐史上最杰出、最成功的艺人之一，迄今发行约30个人专辑累积销售量早在1998年由《TVBS周刊》调查已突破1千3百万张，有华语乐坛“东方不败”美称。",
                    "img": "http://image.kaolafm.net/mz/images/201410/cc1ed246-6743-4f19-9a9a-784d3245b31b/default.jpg"
                }
            ],
            "albumDescription": "",
            "description": "泪滴泪滴　在我的眼里　从来不肯轻易的留下痕迹\r\n泪滴泪滴　在我的眼里　请你请你请你不要再离去\r\n浓浓愁绪　怎能说明　请你不要离去\r\n\r\n黎明里的浓雾渐渐散去\r\n你握著我的手说就要分离\r\n再也没有甜蜜的相聚　不会再说此情不渝\r\n\r\n当你的身影逐渐的远离\r\n只能告诉自己忘了过去\r\n就当你只是一场幻影　梦醒之后消失踪影",
            "publishDate": "1438015267000",
            "md5": "",
            "rate": "64",
            "number": 1,
            "fileSzie": ""
        },
        {
            "aid": "1000000007381",
            "cover": "http://image.kaolafm.net/mz/images/201404/208876df-c0f6-4e0c-9ff8-aa91c15147c2/default.jpg",
            "albumId": "1100000004525",
            "albumName": "原来",
            "title": "原来",
            "playurl": "http://image.kaolafm.net/mz/mp3_64/201403/a0b1ea9a-161b-40b9-b902-d9477c8ad6ea.mp3?appid=fiaju0644&deviceid=100000029020744&audioid=1000000007381",
            "duration": null,
            "categoryId": "129",
            "clockId": "",
            "intercutTime": "",
            "hostList": [
                {
                    "name": "信乐团",
                    "description": "信乐团堪称台湾乐坛最具代表力与影响力的乐队，他们成立于2002年，发行过多张专辑。初期成员有黄迈可、孙志群、刘晓华、傅超华和苏见信。2007年主唱苏见信离团，信乐团一度暂停活动。2008年10月，信乐团在北京举办主唱征选活动。2009年底，来自贵州的刘文杰加入信乐团成为新任主唱。2011年发行暌违6年的专辑《就是唯一》。",
                    "img": "http://image.kaolafm.net/mz/images/201410/85edf3f0-b462-47b5-9f12-4981c1549109/default.jpg"
                }
            ],
            "albumDescription": "",
            "description": "原来爱不能强求\r\n越想拥有 往往越会得不到\r\n其实我们心里 都知道\r\n\r\n我也只能沉默\r\n看着窗边下着绵绵夜雨\r\n你到底要不要\r\n为何不肯说明了\r\n\r\n我看着你冷冷的微笑\r\n像是对我说这不是我们的幸福\r\n再走下去 是宽容还是结束\r\n都一样残酷\r\n\r\n我到现在终于才明白\r\n我就算赢得了世界也会输给你\r\n你的笑容 原来是最狠的报复\r\n\r\n原来爱不能强求\r\n越想拥有 往往越会得不到\r\n其实我们心里 都知道\r\n\r\n我也只能沉默\r\n看着窗边下着绵绵夜雨\r\n你到底要不要\r\n为何不肯说明了\r\n\r\n我看着你冷冷的微笑\r\n像是对我说这不是我们的幸福\r\n再走下去 是宽容还是结束\r\n都一样残酷\r\n\r\n我到现在终于才明白\r\n我就算赢得了世界也会输给你\r\n你的笑容 原来是最狠的报复\r\n\r\n我已经没有退路 我原来已被你俘虏\r\n爱情原来是你最伤人的毒\r\n\r\n我看着你冷冷的微笑\r\n像是对我说这不是我们的幸福\r\n再走下去 是宽容还是结束\r\n都一样残酷\r\n\r\n我到现在终于才明白\r\n我就算赢得了世界也会输给你\r\n你的笑容 原来是最狠的报复 ",
            "publishDate": "1393821563000",
            "md5": "",
            "rate": "64",
            "number": 1,
            "fileSzie": ""
        },
        {
            "aid": "1000000762319",
            "cover": null,
            "albumId": "1100000037939",
            "albumName": "公益－不做低头族－解放篇",
            "title": "公益－不做低头族－解放篇",
            "playurl": "http://image.kaolafm.net/mz/mp3_64/201411/48810796-25cb-44b0-9b44-05dcbc920c22.mp3?appid=fiaju0644&deviceid=100000029020744&audioid=1000000762319",
            "duration": null,
            "categoryId": "131",
            "clockId": "",
            "intercutTime": "",
            "hostList": [ ],
            "albumDescription": "",
            "description": "",
            "publishDate": "1415704554000",
            "md5": "",
            "rate": "64",
            "number": 1,
            "fileSzie": ""
        },
        {
            "aid": "1000000403376",
            "cover": "http://image.kaolafm.net/mz/images/201409/7c75525f-aaac-4f11-8665-6b2caa201c85/default.jpg",
            "albumId": "1100000022520",
            "albumName": "A Song For You",
            "title": "A Song For You",
            "playurl": "http://image.kaolafm.net/mz/mp3_64/201409/b72b5936-58a4-4a84-aa69-9ff10b3986d0.mp3?appid=fiaju0644&deviceid=100000029020744&audioid=1000000403376",
            "duration": null,
            "categoryId": "129",
            "clockId": "",
            "intercutTime": "",
            "hostList": [
                {
                    "name": "Celine Dion",
                    "description": "席琳·迪翁1968年3月30日生于加拿大魁北克省。1990年推出首张英文专辑《UNISON》。1997年为电影《泰坦尼克号》献唱片尾曲《My Heart Will Go On》，并获得第70届奥斯卡最佳电影歌曲奖。\r\n2001年，席琳成为母亲。2003年复出，2003年3月至2007年12月在拉斯维加斯举行了《新的一天...》演唱会，历时5年共732场。一路走来，她已成为流行音乐世界最闪亮的明星。\r\n席琳·迪翁在全球范围内最少获得146项个人独占的音乐类纪录及非音乐类纪录，当中包括各类奖项、销量、排行榜成绩等，其中部分傲人纪录更是预计后人无法企及和打破！",
                    "img": "http://image.kaolafm.net/mz/images/201410/36862940-7bfc-41a9-b443-886f96a99daa/default.jpg"
                }
            ],
            "albumDescription": "",
            "description": "Whitney , the queen of RnB!\r\n\r\nI've been so many places\r\nIn my life and time\r\nI've sung a lot of songs\r\nAnd I made some bad rhyme\r\n\r\nI've acted out my life in stages\r\nWith ten thousand people watching\r\nWell , but we're alone now\r\nAnd I'm singing this song to you\r\n\r\nI know your image of me\r\nIs what I hope to be\r\nI've treated you unkindly\r\nBut darling can't you see\r\n\r\nThere's no one more important to me\r\nBaby, can't you see through me\r\nWe're alone now\r\nAnd I'm singing this song to you\r\n\r\nYou taught me precious secrets\r\nOf the truth withholding nothing\r\nYou came out in front\r\nWhen I was hiding\r\n\r\nBut now I'm so much better\r\nAnd if my words don't come together\r\nListen to the melody\r\n'Cause my love is in there hiding\r\n\r\nI love you in a place\r\nWhere there's no space or time\r\nI love you for my life\r\nThen you are a friend of mine\r\n\r\nAnd when my life is over\r\nRemember when we were together (together)\r\nWe were alone\r\nAnd I was singing this song for you\r\n\r\nThis song for you\r\nThis song this song\r\nThis song for you\r\nThis song this song\r\nThis song for you\r\nThis song this song\r\nThis song for you you you you........\r\n\r\nI love you in place\r\nMy dear friend , where there's no space or time\r\nI love you for my life\r\nYou are a friend of mine\r\n\r\nAnd when my life is over\r\nRemember when we were together\r\nWe were alone\r\nAnd I was singing this song to you\r\n\r\nSinging this song to you\r\nSinging this song to you\r\nSinging this song\r\nI will sing this song for you",
            "publishDate": "1409811731000",
            "md5": "",
            "rate": "64",
            "number": 1,
            "fileSzie": ""
        },
        {
            "aid": "1000000018719",
            "cover": "http://image.kaolafm.net/mz/images/201403/fd797e07-3ac8-467a-8616-81ec67d609dc/default.jpg",
            "albumId": "1100000006638",
            "albumName": "My All",
            "title": "My All",
            "playurl": "http://image.kaolafm.net/mz/mp3_64/201403/839848c8-5819-48f8-b428-6111b33f412d.mp3?appid=fiaju0644&deviceid=100000029020744&audioid=1000000018719",
            "duration": null,
            "categoryId": "129",
            "clockId": "",
            "intercutTime": "",
            "hostList": [
                {
                    "name": "Mariah Carey",
                    "description": "玛丽亚·凯莉，1970年3月27日出生于美国纽约州长岛。她的母亲是拥有爱尔兰血统的白人歌剧女歌手，父亲则拥有非洲及委内瑞拉血统，因此凯莉常被美国媒体归类于黑人歌手。\r\n凯莉因其2亿张的唱片销量和无数的音乐榜单记录，以及5个八度的高亢音域和R&B式的演唱技巧闻名于世。 \r\n凯莉也被美国媒体誉为90年代至今的跨世纪天后歌手之一。她是全世界歌唱比赛参赛者最爱模仿的歌声，同时也是许多艺人梦寐以求合作的对象，但再多的封号与奖项也不足以形容凯莉的伟大与影响力。2008年凯莉入选《时代》杂志年度世界最有影响力人物之一。\r\n",
                    "img": "http://image.kaolafm.net/mz/images/201410/a904419a-b646-4946-bd50-01733cae1c86/default.jpg"
                }
            ],
            "albumDescription": "",
            "description": "I am thinking of you.\r\nIn my sleepless solitude tonight.\r\nIf its wrong to love you\r\nThen my heart just wont let me be right.\r\nCause Im drowned in you.\r\nAnd I wont pull through.\r\nWithout you by my side.\r\nId give my all to have.\r\nJust one more night with you.\r\nId risk my life to feel.\r\nYour body next to mine.\r\nCause I cant go on.\r\nLiving in the memory of our song.\r\nId give my all for your love tonight\r\nBaby can you feel me?\r\nImagining Im looking in your eyes.\r\nI cant see you clearly.\r\nVividly emblazoned in my mind.\r\nAnd yet you are so far.\r\nLike a distant star.\r\nIm wishing on tonight.\r\nId give my all to have.\r\nJust one more night with you.\r\nId risk my life to feel.\r\nYour body next to mine\r\nCause i cant go on.\r\nLiving in the memory of our song.\r\nId give my all for your love tonight.\r\n[Guitar Break]\r\nId give my all to have.。\r\nJust one more night with you.\r\nId risk my life to feel.\r\nYour body next to mine.\r\nCause I cant go on.\r\nLiving in the memory of our song.\r\nId gi",
            "publishDate": "1396258654000",
            "md5": "",
            "rate": "64",
            "number": 1,
            "fileSzie": ""
        },
        {
            "aid": "1000000007578",
            "cover": "http://image.kaolafm.net/mz/images/201404/34548683-7d37-4605-8438-c2f9f3405570/default.jpg",
            "albumId": "1100000004481",
            "albumName": "孤单爱情海",
            "title": "孤单爱情海",
            "playurl": "http://image.kaolafm.net/mz/mp3_64/201402/99f7896b-64b6-4de1-8832-1ac05fffea39.mp3?appid=fiaju0644&deviceid=100000029020744&audioid=1000000007578",
            "duration": null,
            "categoryId": "129",
            "clockId": "",
            "intercutTime": "",
            "hostList": [
                {
                    "name": "黄品源",
                    "description": "黄品源（1967年3月17日—）台湾歌手，二十岁时与哥哥报名参加“第一届青春之星校际音乐大赛”，初试啼声即获得第二名。之后，他向制作人沈光远自荐自己的创作，而得其赏识，正式与他签约。在台湾，黄品源的专辑总销售量超越一佰万张以上，但其出碟频率颇低。2002年4月，黄品源主持中国电视公司综艺节目《综艺大哥大》是黄品源首度主持电视节目；2010年加盟内地新东家北京百娱国际文化传媒有限公司，期待在内地更大的市场发展空间。",
                    "img": "http://image.kaolafm.net/mz/images/201410/a242eb29-e5e0-4102-b74e-6f81717b83c6/default.jpg"
                }
            ],
            "albumDescription": "",
            "description": "潮起潮落的海浪\r\n 像我思念的心好乱\r\n 失去你就像沉没的船\r\n 如果早一天说爱你\r\n 也许能挽回你的心\r\n 是恨是祝福分不清\r\n 我以为可以\r\n 假装从此不相依\r\n 不在乎不在乎你\r\n 谁说溃啼的泪\r\n 不会太难过\r\n 不想你才是这么\r\n\r\n 我的爱情海下着雨\r\n 谁在夜里哭泣\r\n 好想雨\r\n 给我些时间\r\n 我会好好重新爱一遍\r\n 我的爱情海下着雨\r\n 最孤单的距离\r\n 我相信\r\n 总会有一天\r\n 哪怕在一万年 ",
            "publishDate": "1393602006000",
            "md5": "",
            "rate": "64",
            "number": 1,
            "fileSzie": ""
        },
        {
            "aid": "1000000010712",
            "cover": "http://image.kaolafm.net/mz/images/201404/1d9f24ac-997a-4e3c-a055-49715ad4e7ee/default.jpg",
            "albumId": "1100000005045",
            "albumName": "取名回忆的时光",
            "title": "取名回忆的时光",
            "playurl": "http://image.kaolafm.net/mz/mp3_64/201403/16504ccb-6a52-43f4-b3f4-13ecdee3a98a.mp3?appid=fiaju0644&deviceid=100000029020744&audioid=1000000010712",
            "duration": null,
            "categoryId": "129",
            "clockId": "",
            "intercutTime": "",
            "hostList": [
                {
                    "name": "吴莫愁",
                    "description": "吴莫愁，1992年4月18日出生于黑龙江省齐齐哈尔市龙沙区，中国大陆新生代个性歌手。吴莫愁从小跟随父母亲开大篷车畅游全国，2012年在《中国好声音》节目中凭借出色表现获得年度亚军，一举成名。2012年与庾澄庆合作单曲《我要给你》，年末荣获中国魅力50人、亚洲年度新锐歌手、年度艺人、全球最美50新人、年度女性榜样等奖项。",
                    "img": "http://image.kaolafm.net/mz/images/201410/4685f317-40cf-4205-ae5f-3d2ed9743805/default.jpg"
                }
                
    ],
    "requestId": "fiaju06440.1143935175219963"

}
###错误信息

请参考错误代码释义
