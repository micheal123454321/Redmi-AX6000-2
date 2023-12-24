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
开启
使用 Meta 内核
运行模式 Fake-IP（TUN-混合）模式【UDP-TUN，TCP-转发】

自定义上游DNS，NameServer只需要填上一个或两个运营商分配的DNS即可
清空 FallBack 跟 Default-NameServer 所有DNS

Fake-IP 持久化

允许解析 IPv6 类型的 DNS 请求

自动更新 GeoIP Dat 数据库
自动更新 GeoSite 数据库

自动更新 大陆白名单

启用流量（域名）探测
探测（嗅探）纯 IP 连接
自定义流量探测（嗅探）设置
```

