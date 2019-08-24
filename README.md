# resetos
当我们需要重装VPS/云平台/独立服务器操作系统时，通常可以通过服务商模板和ISO挂载的方式重新安装。

从今天开始，你将拥有了一个全新的方式，通过网络一键式重新安装纯净操作系统，无需CD-ROM,无需VNC/IPIM/KVM。

无论是Linux，还是Windows，都可以通过网络一键式完成安装，通过简单的两行命令开启美妙的体验。

现实需求
为什么我们需要重装纯净系统？

1. 服务商提供的系统模板可能会内置一些软件，甚至和我们即将安装的软件产生冲突，导致安装失败。

2. ISO挂载并不是所有服务商都提供的服务，一些IPIM/KVM传输速度过于缓慢，安装效率较差。

3. Linux/Windows在使用中可能遇到一些找不到问题的莫名错误。相信你一定深有体会！

你需要了解
1. 所有系统除特殊说明外，安装完毕的默认密码是cxthhhhh.com，为了防止暴力破解，你必须在安装完毕立刻修改默认密码！

2. 因硬件配置和网络环境不同，安装全程需要15-60分钟，请耐心等待。安装完成即可通过IP:22(Linux SSH)/IP:3389(Windows RDP)进行连接。

3. 为了稳定性和安全性，我建议所有网站管理员/开发者/公司使用最新的系统，同时我只为最新的系统提供技术支持。

4. 一些没有DHCP的VPS/云平台/独立服务器，安装后无法访问网络，你需要登陆VNC/IPIM/KVM后手动进行网卡IP配置。

 

重装系统前环境需求
1. 当前已安装任意由GRUB or GRUB2引导Linux系统(RedHat/CentOS/Debian/Ubuntu/Etc.)

2. 安装重装系统的前提组件

①. RedHat/CentOS:

yum install -y xz openssl gawk file
②. Debian/Ubuntu:

apt-get install -y xz-utils openssl gawk file
让我们开始吧


1. 下载SHELL脚本（通过root用户运行）
```
wget --no-check-certificate https://shell.p1e.cn/reinstall/Network-Reinstall-System-Modify.sh && chmod a+x Network-Reinstall-System-Modify.sh
```
