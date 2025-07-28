地址: **192.168.6.1**<br>
用户名: **root**<br>
密码: **password**


**OpenClash 设置**
```
**插件设置**

✅ 使用 Meta 内核
运行模式 Fake-IP（TUN-混合）模式【UDP-TUN，TCP-转发】

✅ 网络栈类型 Mixed（仅 Meta 内核）


✅ 路由本机代理
✅ 禁用 QUIC
✅ 绕过服务器地址
仅允许常用端口流量 禁用

✅ 本地 DNS 劫持 使用 Dnsmasq 转发
✅ 禁止 Dnsmasq 缓存 DNS

✅ IPv6 流量代理
✅ IPv6 代理模式 Mix 混合模式【UDP-TUN，TCP-转发】（仅 Meta 内核）
✅ 允许解析 IPv6 类型的 DNS 请求

✅ 自动更新 GeoIP Dat 数据库
✅ 自动更新 GeoSite 数据库
✅ 自动更新 大陆白名单


**覆写设置**

Github 地址修改 https://testingcf.jsdelivr.net/

✅ 自定义上游 DNS 服务器
✅ Fake-IP 持久化
✅ Fake-IP-Filter
✅ Fake-IP-Filter-Mode 黑名单模式


✅ Nameserver-Policy
"geosite:!cn":
    - tls://1.1.1.1#⚡️ 国际代理
    - tls://8.8.8.8#⚡️ 国际代理

✅ NameServer
   - 223.5.5.5

✅ FallBack
- tls://dns.google
- tls://1.1.1.1



✅ 启用 TCP 并发
❌ Geodata 数据加载方式 禁用
✅ 启用 GeoIP Dat 版数据库
✅ 启用流量（域名）探测
✅ 探测（嗅探）纯 IP 连接
✅ 自定义流量探测（嗅探）设置

手动更新为 mihomo 内核 mihomo-linux-arm64-v1.19.2.gz
支持 Hysteria2节点

✅  DHCP/DNS  DNS 重定向 重定向客户端DNS到dnsmasq

```
**IPV6 设置**
```
✅ 删除 全局网络选项 » IPv6 ULA 前缀

接口 » LAN » 高级设置
✅  委托 IPv6 前缀
   IPv6 分配长度 64

接口 » LAN » DHCP 服务器
✅ RA 服务 服务器模式
❌ DHCPv6 服务 已禁用
❌ 本地 IPV6 DNS 服务器
❌ NDP 代理 已禁用

接口 » LAN » DHCP 服务器 » IPv6 RA 设置
✅ 启用 SLAAC
✅ RA 标记 无

```
