##版本升级接口
===
###请求方式
---

**GET** `http://open.kaolafm.com/v1/app/version?appid={appid}&sign={sign}&openid={openid}&version={version}`

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
| version   | string |   是   |当前版本号


###返回参数
---

| 参数名称 | 类型    | 描述 
|:------- |-------:|:------:|
| updateType   | int |   升级类型  |
| updateVersion  | string |   升级版本号 |
|updateInfo|string|升级信息
|updateUrl|string|apk下载地址





###结果样例
---

    {

    "result": {
		"updateType": 1,
		"updateVersion": "1.1.0",
		"updateInfo": "1.新增【订阅】功能\n2.修复已知问题，优化体验\n",
		"updateUrl": "http://open.kaolafm.com/kaolafm.apk"
	},
	"requestId": "ffzex14030.11461045291564626"

    }

###错误信息

请参考错误代码释义
