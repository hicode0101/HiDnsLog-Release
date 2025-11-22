# HiDnsLog-Release
Release HiDnsLog




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
