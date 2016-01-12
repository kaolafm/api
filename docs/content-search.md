##搜索指定关键字内容
===
###请求方式
---

**GET** `http://open.kaolafm.com/v1/content/search?appid={appid}&sign={sign}&openid={openid}&q={q}&page={page}&size={size}`

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
| q   | string |   是   |搜索关键词
| types    | string |   否   |内容类型(0:专辑 1:碎片 3:电台 ) 多个类型使用,间隔如 0,1
| page    | string |   否   |页数 默认为1
| size | string | 否 | 每页数据条数 默认为10 最大50

###返回参数
---

| 参数名称 | 类型    | 描述 
|:------- |-------:|:------:|
| cid   | string |   内容id  |
| type    | string |   内容类型(0:专辑 1:碎片 3:电台 )   |
| name  | string |   名称 |
|img|string|封面
|description|string|内容描述
|categoryId|string|分类id 详见[媒体类型分类](mztypes.md)
|categoryName|string|分类名称
|分页字段
|total|string|	记录总数
|prev|string|上一页 无上一页输出 -1
|next|string|下一页 无下一页输出 -1


###结果样例
---

    {
    "result": {
    "total": "36",
    "next": "2",
    "prev": "-1",
    "list": [
      {
        "cid": "1100000000134",
        "name": "头条新闻",
        "img": "http://image.kaolafm.net/mz/images/201411/1e98d14e-8451-4c96-ad40-b781bd089527/default.jpg",
        "description": "聚焦重大新闻，还原事实真相",
        "type": "0",
        "categoryId": "116",
        "categoryName": "资讯"
      },
      {
        "cid": "1100000000058",
        "name": "V言耸听",
        "img": "http://image.kaolafm.net/mz/images/201406/142eb56f-1c95-4360-a25b-98c13286bb6e/default.jpg",
        "description": "微：微天下；言：语言犀利 言之有物；耸：大V发声 挺拔耸立 观点明晰；听：带您倾听更直观的世界。这里是聚焦时事热点，聆听大V点评的考拉微言耸听",
        "type": "0",
        "categoryId": "116",
        "categoryName": "资讯"
      },
      {
        "cid": "1100000000279",
        "name": "新闻7点整",
        "img": "http://image.kaolafm.net/mz/images/201409/0d4681cc-bded-4692-a2f1-cd06513ae082/default.jpg",
        "description": "这里有最严肃的新闻，这里有最调侃的语言，尽在《新闻7点整》，每天听尽天下事。",
        "type": "0",
        "categoryId": "116",
        "categoryName": "资讯"
      }
    ]
    },
    "requestId": "zcrzd94051416464578806827"
    }    


###错误信息

请参考错误代码释义
