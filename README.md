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
使用 Meta 内核
运行模式 Fake-IP（TUN-混合）模式【UDP-TUN，TCP-转发】

绕过中国大陆 IPv4 黑名单
##解决绕过大陆后谷歌商店无法更新
#services.googleapis.cn


使用 Dnsmasq 转发
禁止 Dnsmasq 缓存 DNS


自定义上游DNS，NameServer只需要填上一个运营商分配的DNS即可
清空 FallBack 跟 Default-NameServer 所有DNS


允许解析 IPv6 类型的 DNS 请求

自动更新 GeoIP Dat 数据库
自动更新 GeoSite 数据库

自动更新 大陆白名单
```

