地址: **192.168.6.1**<br>
用户名: **root**<br>
密码: **password**


**Redmi-AX6000-hanwckf**
```
luci-app-filetransfer
luci-app-firewall
luci-app-mtk
luci-app-opkg
luci-app-turboacc-mtk
luci-theme-argon
luci-theme-bootstrap
luci-app-openclash + 全部内核 + GeoIP 数据库 + GeoSite 数据库
```


**OpenClash 设置**
```
FakeIP增强模式 + Meta内核，自定义DNS只留两个NameServer填运营商的DNS

Fake-IP 持久化，启用流量（域名）探测，探测（嗅探）纯 IP 连接，自定义流量探测（嗅探）设置把这几个功能开启
```


**OpenClash rules规则**
```
; 谷歌商店下载
ruleset=🚀 节点选择,[]DOMAIN-SUFFIX,xn--ngstr-lra8j.com
ruleset=🚀 节点选择,[]DOMAIN-SUFFIX,services.googleapis.cn

; 内网IP，匹配上走直连，不发起DNS请求
ruleset=🎯 全球直连,[]GEOIP,private,no-resolve

; 内网地址，匹配上的走直连
ruleset=🎯 全球直连,[]GEOSITE,private

; 国内域名，匹配上的走直连
ruleset=🎯 全球直连,[]GEOSITE,CN

; 国内基于IP的地址，匹配上走直连，不发起DNS请求
ruleset=🎯 全球直连,[]GEOIP,CN,no-resolve

; 兜底，都没匹配上就走代理
ruleset=🌐 代理终端,[]FINAL
```
