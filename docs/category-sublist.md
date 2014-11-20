##获取指定分类下列表
===
###请求方式
---

**GET** `http://open.kaolafm.com/v1/category/sublist?appid={appid}&sign={sign}&openid={openid}&cid={cid}`

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
| cid   | string |   否   |分类id（不填输出应用所有分类）
| source    | string |   否   |分类来源 （0：专辑 1：电台）

###返回参数
---

| 参数名称 | 类型    | 描述 
|:------- |-------:|:------:|
| cid   | string |   分类id  |
| name    | string |   分类名称  |
| hasSub  | string |   是否有下级分类（0：否 1：是）  |
|logo|string|logo
###结果样例
---

    {

    "result": [
        {
            "cid": "540",
            "name": "健康读物",
            "type": "0",
            "logo": "http://image.kaolafm.net/mz/images/201411/58e2b956-8a02-4184-8769-e13e867530dd/default.jpg",
            "hassub": "0"
        },
        {
            "cid": "539",
            "name": "儿童读物",
            "type": "0",
            "logo": "http://image.kaolafm.net/mz/images/201411/ad3419eb-9844-4916-a8d4-0e8bee35b0b2/default.jpg",
            "hassub": "0"
        },
        {
            "cid": "538",
            "name": "评书",
            "type": "0",
            "logo": "http://image.kaolafm.net/mz/images/201411/3b748f31-8825-4fb4-ba11-73217f66584e/default.jpg",
            "hassub": "0"
        },
        {
            "cid": "532",
            "name": "新闻",
            "type": "1",
            "logo": "http://image.kaolafm.net/mz/images/201411/af52f01e-192c-49dd-86ea-62ba10a428a5/default.jpg",
            "hassub": "0"
        },
        {
            "cid": "476",
            "name": "相声",
            "type": "0",
            "logo": "http://image.kaolafm.net/mz/images/201411/3371b784-31a9-4df3-83c7-421d6be18715/default.jpg",
            "hassub": "0"
        }
    ],
    "requestId": "zcrzd94051416454327033600"
    }
    


###错误信息

请参考错误代码释义