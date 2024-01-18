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
*运行模式Fake-IP（增强）模式
UDP 流量转发

使用 Dnsmasq 转发
禁止 Dnsmasq 缓存 DNS


自定义上游DNS，NameServer只需要填上一个或两个运营商分配的DNS即可
清空 FallBack 跟 Default-NameServer 所有DNS


IPv6 设置
IPv6 流量代理
IPv6 代理模式  TProxy 模式
UDP 流量转发
允许解析 IPv6 类型的 DNS 请求

自动更新 GeoIP Dat 数据库
自动更新 GeoSite 数据库

自动更新 大陆白名单
```

