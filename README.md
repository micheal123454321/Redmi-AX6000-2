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
luci-app-upnp
luci-theme-argon
luci-theme-bootstrap
luci-app-openclash + 全部内核 + GeoIP 数据库 + GeoSite 数据库
```

**OpenClash 设置**
```
【勾选】，使用 Meta 内核
【切换】运行模式 Fake-IP（增强）模式

【取消】，UDP 流量转发

绕过中国大陆 IPv4 黑名单
##解决绕过大陆后谷歌商店无法更新
#services.googleapis.cn

使用 Dnsmasq 转发
【勾选】，禁止 Dnsmasq 缓存 DNS

清空 NameServer、FallBack、Default-NameServer 所有DNS
【勾选】，Nameserver-Policy 填入：'GEOSITE:cn': '223.6.6.6'

【勾选】，自定义上游DNS，NameServer只需要填入：doh.apad.pro/dns-query，服务器类型选择：HTTPS

【勾选】，允许解析 IPv6 类型的 DNS 请求

【勾选】，自动更新 GeoIP Dat 数据库
【勾选】，自动更新 GeoSite 数据库

【勾选】，自动更新 大陆白名单

【取消】，启用流量（域名）探测

```

