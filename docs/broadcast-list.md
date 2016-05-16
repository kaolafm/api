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


###错误信息

请参考错误代码释义

