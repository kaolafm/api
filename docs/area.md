##获取电台地区接口
===
###请求方式
---

**GET** `http://open.kaolafm.com/v1/broadcast/area?appid={appid}&sign={sign}&openid={openid}`

###认证参数
---
| 参数名称 | 类型    | 是否必需 |描述
|:------- |-------:|:------:|:----|
| appid   | string |   是   |应用id
| sign    | string |   是   |签名
| openid  | string |   是   |设备标识


###请求参数
---
无


###返回参数
---

| 参数名称 | 类型    | 描述 
|:------- |-------:|:------:|
| id   | int | 地区code  |
| name  | string |   名称 |
###结果样例
---
```
{
result: [
{
id: 1,
name: "北京"
},
{
id: 20,
name: "重庆"
},
{
id: 28,
name: "上海"
},
{
id: 2,
name: "天津"
},
{
id: 12,
name: "安徽"
},
{
id: 25,
name: "福建"
},
{
id: 26,
name: "广东"
},
{
id: 17,
name: "甘肃"
},
{
id: 27,
name: "广西"
},
{
id: 23,
name: "贵州"
},
{
id: 7,
name: "河北"
},
{
id: 21,
name: "湖北"
},
{
id: 8,
name: "河南"
},
{
id: 22,
name: "湖南"
},
{
id: 31,
name: "海南"
},
{
id: 6,
name: "黑龙江"
},
{
id: 3,
name: "吉林"
},
{
id: 13,
name: "江苏"
},
{
id: 11,
name: "江西"
},
{
id: 29,
name: "辽宁"
},
{
id: 4,
name: "内蒙"
},
{
id: 18,
name: "宁夏"
},
{
id: 30,
name: "青海"
},
{
id: 19,
name: "四川"
},
{
id: 10,
name: "山东"
},
{
id: 9,
name: "山西"
},
{
id: 5,
name: "陕西"
},
{
id: 24,
name: "云南"
},
{
id: 15,
name: "浙江"
},
{
id: 14,
name: "新疆"
},
{
id: 16,
name: "西藏"
},
{
id: 33,
name: "澳门"
},
{
id: 34,
name: "香港"
},
{
id: 32,
name: "台湾"
}
],
requestId: "ffzex14032.2331463455455967508"
}
```
