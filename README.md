### 自己配置文件地址: https://gitee.com/fengymi/gfwlist/raw/master/myself_gfwlist_base

<br/>

[链接文档](https://iangeli.com/2017/08/08/Shadowsocks-PAC.html)

<p/>

[原始文档](https://adblockplus.org/en/filter-cheatsheet)

<br/>

user-rule文件的语法规则
user-rule文件中，每一行表示一个URL通配符，但是通配符语法类似。例如添加一行 ||ip138.com^
注意末尾不要忘记 ^ 符号，意思是要么在这个符号的地方结束，要么后面跟着?,/等符号。
自定义代理规则的设置语法与GFWlist相同，语法规则如下：
1. 通配符支持。比如 .example.com/ 实际书写时可省略 * ， 如 .example.com/ ， 和 .example.com/ 效果一样
2. 正则表达式支持。以 \ 开始和结束， 如 [\w]+:\/\/example.com\
3. 例外规则 @@ ，如 @@.example.com/ 满足 @@ 后规则的地址不使用代理
4. 匹配地址开始和结尾 | ，如 |http://example.com 、 example.com| 分别表示以 http://example.com 开始和以 example.com 结束的地址
5. || 标记，如 ||example.com 则 http://example.com 、 https://example.com 、 ftp://example.com 等地址均满足条件
6. 注释 ! 。 如 !我是注释

## 小火箭规则 <br />
[参考文档](https://jiuaidu.com/jianzhan/931464/)
![image小火箭规则.png](iamges%2Fimage%E5%B0%8F%E7%81%AB%E7%AE%AD%E8%A7%84%E5%88%99.png)



## V2ray规则 <br />
https://www.v2fly.org/config/routing.html#ruleobject
![v2ray路由规则.png](iamges%2Fv2ray%E8%B7%AF%E7%94%B1%E8%A7%84%E5%88%99.png)