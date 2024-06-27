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
【取消勾选】UDP 流量转发

【勾选】，绕过服务器地址

 WAN 接口名称 eth1

 使用 Dnsmasq 转发
【勾选】，禁止 Dnsmasq 缓存 DNS

【勾选】，允许解析 IPv6 类型的 DNS 请求

【勾选】，自动更新 GeoIP Dat 数据库
【勾选】，自动更新 GeoSite 数据库

Github 地址修改 https://testingcf.jsdelivr.net/

TCP Keep-alive 间隔（s）1800

【勾选】，自定义上游 DNS 服务器
【勾选】，追加上游 DNS
【勾选】，Fake-IP 持久化

  清空 NameServer、FallBack、Default-NameServer 所有DNS


【勾选】，自动更新 GeoIP Dat 数据库
【勾选】，自动更新 GeoSite 数据库

【勾选】，自动更新 大陆白名单

【取消】，启用流量（域名）探测

```

