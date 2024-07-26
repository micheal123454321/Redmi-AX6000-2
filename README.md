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

运行模式 Fake-IP（增强）模式
【勾选】UDP 流量转发

 使用 Dnsmasq 转发
【勾选】，禁止 Dnsmasq 缓存 DNS

【勾选】，允许解析 IPv6 类型的 DNS 请求

【勾选】，自动更新 GeoIP Dat 数据库
【勾选】，自动更新 GeoSite 数据库

Github 地址修改 https://testingcf.jsdelivr.net/

【勾选】，自定义上游 DNS 服务器
【勾选】，Fake-IP 持久化

  清空 NameServer、FallBack、Default-NameServer 所有DNS

在NameServer填入一个营运营商DNS

【勾选】，自动更新 GeoIP Dat 数据库
【勾选】，自动更新 GeoSite 数据库

【勾选】，自动更新 大陆白名单

【取消】，启用流量（域名）探测
【勾选】，启用 GeoIP Dat 版数据库
```
**IPV6 设置**
```
删除 全局网络选项 » IPv6 ULA 前缀

接口 » LAN » 高级设置
【取消】委托 IPv6 前缀
IPv6 分配长度 64

接口 » LAN » DHCP 服务器
RA 服务 服务器模式
DHCPv6 服务 已禁用
【取消】本地 IPV6 DNS 服务器
NDP 代理 已禁用

接口 » LAN » DHCP 服务器 » IPv6 RA 设置
启用 SLAAC
RA 标记 无

接口 » WAN6 » 高级设置
【取消】IPv6 源路由
```
