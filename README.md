# HiDnsLog-Release
Release HiDnsLog

```

一个可查询和管理DNS解析记录的工具，支持DNSlog 私有化部署，即使用自己的域名。

支持完整的DNS Server 功能，支持自动从其它DNS Server返回解析记录。

目前支持 A、AAAA、CNAME、MX、TXT 记录，白帽子师傅完全够用。

支持域名解析自动二次绑定（绕过一些检测）。

支持TTL 设置为 0，这是白帽必备功能，且几乎所有域名服务商都不支持，所以要用自己的。

支持 A记录、CNAME记录的重绑定，并且支持指定重绑定的解析顺序，一切尽在你的掌控中，无需大量随机碰撞。

*支持SSRF跳转漏洞测试，支持Burp Collaborator。


```



安装部署详细教程下周抽时间补上，先简单说一下安装步骤：
```
运行方式1：直接运行服务
./hidnslog_linux_amd64


运行方式2：安装成服务
./hidnslog_linux_amd64 install

启动服务
service hidns start

停止服务
service hidns stop

查看服务状态
service hidns status

如果后期需要删除服务，可执行下面命令：
./hidnslog_linux_amd64 uninstall


启动成功后，用浏览器直接访问web控制台：
http://你的IP:8053
初始用户名：hidns
初始密码：123456

进入系统后请第一时间修改密码，切记。
```

然后把你自己的域名解析到服务商那边改到你自己的部署的服务器IP就可以了，需要两个NS，防火墙要开 UDP 协议的 53端口。

具体使用细节也可以群里面直接问我。

来张图：
<img src="ScreenShot/screen-1.png" width="900" />
