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
FakeIP增强模式 + Meta内核
自定义DNS只留一个NameServer填运营商DNS

允许解析 IPv6 类型的 DNS 请求
自动更新 GeoIP Dat 数据库
自动更新 GeoSite 数据库
Fake-IP 持久化

关闭
启用流量（域名）探测
探测（嗅探）纯 IP 连接
```

