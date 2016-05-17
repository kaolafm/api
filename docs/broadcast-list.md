##获取传统电台列表
===
###请求方式
---

**GET** `http://open.kaolafm.com/v1/broadcast/list?appid={appid}&sign={sign}&openid={openid}&classfyid={classfyid}&code={code}&page={page}&pagesize={pagesize}`

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
| classfyid   | int |   是   |分类id 1 国家台 2 省市台 3 网络台
| code   | int |   否   | 城市code 
| page    | string |   否   |页数 默认为1
| pagesize | string | 否 | 每页数据条数 默认为50 最大50

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
|分页字段
|page|int|	当前页码
|pagesize|int|每页显示多少条
|count|int|总条数
|totalPages|int|总页数


###结果样例
---

 { 
result: { 
page: 1, 
pageSize: 10, 
count: 17, 
totalPages: 2, 
haveNext: 1, 
nextPage: 2, 
havePre: 0, 
prePage: 1, 
startNum: 0, 
endNum: 10, 
dataList: [{ 
id: 1600000000510, 
name: “央广中国之声”, 
desc: “中国唯一覆盖全国的24小时新闻直播频率。”, 
pic: “http://image.kaolafm.net/mz/images/201512/80b53c48-fc67-4ab8-9ebc-a68dc3654419/default.jpg“, 
playUrl: “http://trslbs.kaolafm.com/016f63815d64d4db/1600000000510/playlist.m3u8“, 
classifyId: 1, 
code: null 
}, 
{ 
id: 1600000000514, 
name: “央广经济之声”, 
desc: “中央人民广播电台经济之声是中国最有影响力的财经广播，立足于“国家级现代传媒机构”的定位，传播全球最新财经资讯，引领经济话语，是中国最具成长性的专业财经媒体。 “, 
pic: “http://image.kaolafm.net/mz/images/201512/c48e2404-dbc9-4803-9599-ec47eedcddb9/default.jpg“, 
playUrl: “http://trslbs.kaolafm.com/016f63815d64d4db/1600000000514/playlist.m3u8“, 
classifyId: 1, 
code: null 
}, 
{ 
id: 1600000000323, 
name: “中国高速公路交通广播”, 
desc: “中央人民广播电台高速公路交通广播，最及时的路况、最新鲜的资讯…”, 
pic: “http://image.kaolafm.net/mz/images/201512/61e5e3a5-f726-456c-86c0-93eb9137c804/default.jpg“, 
playUrl: “http://trslbs.kaolafm.com/016f63815d64d4db/1600000000323/playlist.m3u8“, 
classifyId: 1, 
code: null 
}, 
{ 
id: 1600000000326, 
name: “央广神州之声”, 
desc: ” 神州之声是中央人民广播电台对台湾广播方言文艺频率。每天分别用普通话、闽南话、客家话播出，沟通两岸亲情…”, 
pic: “http://image.kaolafm.net/mz/images/201512/c0469ea2-b5df-490b-983f-7968d3de4b84/default.jpg“, 
playUrl: “http://trslbs.kaolafm.com/016f63815d64d4db/1600000000326/playlist.m3u8“, 
classifyId: 1, 
code: null 
}, 
{ 
id: 1600000000327, 
name: “央广文艺之声”, 
desc: “全天候的文化资讯、直击北京及全国文化市场，为主流收听群体服务，打造高品质的文化生活；我们传播文化精髓，引导人们的文化生产与消费生活。”, 
pic: “http://image.kaolafm.net/mz/images/201512/3e9470bd-50a5-4bf0-a07f-800ba1c96fb3/default.jpg“, 
playUrl: “http://trslbs.kaolafm.com/016f63815d64d4db/1600000000327/playlist.m3u8“, 
classifyId: 1, 
code: null 
}, 
{ 
id: 1600000000513, 
name: “央广都市之声”, 
desc: “youRadio 都市之声FM101.8是中央人民广播电台旗下覆盖北京的都市生活电台，致力于打造“北京生活手册” ，服务首都百姓生活。”, 
pic: “http://image.kaolafm.net/mz/images/201512/9c7fc622-7b9c-41e6-9a39-0338aef36941/default.jpg“, 
playUrl: “http://trslbs.kaolafm.com/016f63815d64d4db/1600000000513/playlist.m3u8“, 
classifyId: 1, 
code: null 
}, 
{ 
id: 1600000000330, 
name: “央广中华之声”, 
desc: “央广中华之声”, 
pic: “http://image.kaolafm.net/mz/images/201512/95392067-07e8-4d12-b36d-091c20078605/default.jpg“, 
playUrl: “http://trslbs.kaolafm.com/016f63815d64d4db/1600000000330/playlist.m3u8“, 
classifyId: 1, 
code: null 
}, 
{ 
id: 1600000000515, 
name: “央广民族之声”, 
desc: “民族之声是中央人民广播电台针对民族地区播出的广播频率，采用蒙古、维吾尔、哈萨克、朝鲜4种民族语言播出，其电波主要覆盖中国内蒙古、新疆、吉林、辽宁、黑龙江及首都北京等地。”, 
pic: “http://image.kaolafm.net/mz/images/201512/f5adad4d-a778-486c-87fd-4aa998777383/default.jpg“, 
playUrl: “http://trslbs.kaolafm.com/016f63815d64d4db/1600000000515/playlist.m3u8“, 
classifyId: 1, 
code: null 
}, 
{ 
id: 1600000000604, 
name: “央广维语广播”, 
desc: “央广维语广播”, 
pic: “http://image.kaolafm.net/mz/images/201601/349ce337-a44f-4892-8b62-6b07422ddeb2/default.jpg“, 
playUrl: “http://trslbs.kaolafm.com/016f63815d64d4db/1600000000604/playlist.m3u8“, 
classifyId: 1, 
code: null 
}, 
{ 
id: 1600000000605, 
name: “央广哈语广播”, 
desc: “央广哈语广播”, 
pic: “http://image.kaolafm.net/mz/images/201601/72338b25-0f3b-403a-a6c9-50d833f2d3a4/default.jpg“, 
playUrl: “http://trslbs.kaolafm.com/016f63815d64d4db/1600000000605/playlist.m3u8“, 
classifyId: 1, 
code: null 
}] 
}, 
requestId: “ffzex14032.2331463380619840988” 
}


###错误信息

请参考错误代码释义

