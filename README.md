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
luci-app-ttyd
luci-app-openclash + 全部内核 + GeoIP 数据库 + GeoSite 数据库
```

**OpenClash 设置**
```
**插件设置**

☑ 使用 Meta 内核
   运行模式 Fake-IP（增强）模式
☑ UDP 流量转发

☑ 绕过服务器地址
☑ 仅允许内网
   WAN 接口名称 eth1

本地 DNS 劫持 使用防火墙转发


☑ IPv6 流量代理
   IPv6 代理模式 TProxy 模式
☑ UDP 流量转发
☑ 允许解析 IPv6 类型的 DNS 请求

☑ 自动更新 GeoIP Dat 数据库
☑ 自动更新 GeoSite 数据库

☑ 自动更新 大陆白名单


**覆写设置**

Github 地址修改 https://testingcf.jsdelivr.net/

☑ 自定义上游 DNS 服务器
  清空 NameServer、FallBack、Default-NameServer 所有DNS
  NameServer填入一个营运商DNS

☑ Fake-IP 持久化

☑ 启用 TCP 并发
   TCP Keep-alive 间隔（s）1800
☑ 启用 GeoIP Dat 版数据库
☒ 启用流量（域名）探测
☒ 探测（嗅探）纯 IP 连接

覆写设置 开发者选项 #27
ruby_edit "$CONFIG_FILE" "['experimental']" "{'sniff-tls-sni'=>false}"

```
**IPV6 设置**
```
删除 全局网络选项 » IPv6 ULA 前缀

接口 » LAN » 高级设置
☒ 委托 IPv6 前缀
   IPv6 分配长度 64

接口 » LAN » DHCP 服务器
RA 服务 服务器模式
DHCPv6 服务 已禁用
☒ 本地 IPV6 DNS 服务器
NDP 代理 已禁用

接口 » LAN » DHCP 服务器 » IPv6 RA 设置
启用 SLAAC
RA 标记 无

接口 » WAN6 » 高级设置
☒ IPv6 源路由
```
