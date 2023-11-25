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
ruleset=🎯 全球直连,[]GEOSITE,cn

; 国内基于IP的地址，匹配上走直连，不发起DNS请求
ruleset=🎯 全球直连,[]GEOIP,cn,no-resolve

; 兜底，都没匹配上就走代理
ruleset=🌐 代理终端,[]FINAL

custom_proxy_group=🚀 节点选择`select`[]🇭🇰 香港-自动`[]🇸🇬 狮城-自动`.*
custom_proxy_group=🎯 全球直连`select`[]DIRECT`[]🚀 节点选择
; custom_proxy_group=🛑 隐私拦截`select`[]REJECT`[]DIRECT
custom_proxy_group=🌐 代理终端`select`[]🚀 节点选择`[]🎯 全球直连

;自动测速
custom_proxy_group=🇭🇰 香港-自动`url-test`(港|HK|Hong Kong)`https://www.gstatic.com/generate_204`600,,50
custom_proxy_group=🇸🇬 狮城-自动`url-test`(新加坡|坡|狮城|SG|Singapore)`https://www.gstatic.com/generate_204`600,,50


enable_rule_generator=true
overwrite_original_rules=true
;skip_failed_links=true

#过滤节点，正则匹配
exclude_remarks=(IPV6|重置|流量|用户|本站|漏洞|永久虚通路|车|邀|免翻|邀请|eevpn|域名|机场|刷新|禁止|备用登录|计划|面板|忘记|到期|套餐|官网|更多|关注|25倍率|http|增加|持续|渠道|购买|QQ|Ins|二手)

;luck
Comment

```
