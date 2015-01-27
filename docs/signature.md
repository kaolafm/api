##签名算法

1. 获取请求的http method;
2. 获取请求的url,包括host和sheme,但不包括query_string的部分;
3. 将http method和url按顺序拼接成新字符串;
4. 在拼接好的字符串末尾追加上应用的secret_key(全部小写),并进行urlencode(将字符串以 URL 编码，编码格式为utf8), 形成 base_string(全部小写);<br>
5. 注：请将UTF-8编码后的所有字母改成小写字母后再进行MD5编码;


**上述字符串的 md5 值（32位）即为签名的值（请把MD5后的字母变为小写）:**

**ex:** sign=md5(urlencode($http_method$url$appid$secret_key),'utf-8');


**例如:**<br>
appid: cntkg4748


secret key: 8cd734379145a43e3f18d5b03f871508


http: get http://open.kaolafm.com/v1/category/sublist?cid=100


**签名方式为** sign = md5(urlencode(gethttp://open.kaolafm.com/v1/category/sublistcntkg47488cd734379145a43e3f18d5b03f871508),utf-8)
￼


