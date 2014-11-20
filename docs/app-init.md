##应用初始化
===
**调用场景**

 1. 每次加载应用时
 2. openid丢失时
 
###请求方式
---

**POST** `http://open.kaolafm.com/v1/app/init`

###认证参数
---
| 参数名称 | 类型    | 是否必需 |描述
|:------- |-------:|:------:|:----|
| appid   | string |   是   |应用id
| sign    | string |   是   |签名


###请求参数
---

| 参数名称 | 类型    | 是否必需 |描述
|:------- |-------:|:------:|:----|
| deviceid  | string |   是   |设备唯一id（可使用手机udid,mac地址,vin等）
| devicetype | string | 是 | 设备类型（0：android 1:ios 2:html5 3:windowsphone）
| osversion| string | 是|操作系统版本
| network |string|是|网络情况（-1：未知 0:无网 1:wifi 2:2G 3:3G 4:4G）
| imsi | string | 否 | sim卡信息
| lon | string | 否 | 经度
| lat | string | 否 | 纬度
| speed | string | 否 | 速度 
| datetime|string | 否 |时间戳格式 yyyyMMddHHmmss 如20140101121212

###返回参数
---

| 参数名称 | 类型    | 描述 
|:------- |:-------:|:------|
| openid   | string |   标识指定设备的标识  |

###结果样例
---
    {
      "result": {
          "openid": "100000017370150"
      },
      "requestId": "zcrzd94051416455268317671"
    }

    


###错误信息

请参考错误代码释义