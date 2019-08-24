参考
https://www.815494.com/html/734.html

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
2. 安装系统（任选其一）
【安装Linux系统】

①. 一键网络重装纯净CentOS 7（推荐）

bash Network-Reinstall-System-Modify.sh -CentOS_7
②. 一键网络重装纯净CentOS 6

bash Network-Reinstall-System-Modify.sh -CentOS_6
③. 一键网络重装纯净Debian 9（推荐）

bash Network-Reinstall-System-Modify.sh -Debian_9
④. 一键网络重装纯净Debian 8

bash Network-Reinstall-System-Modify.sh -Debian_8
⑤. 一键网络重装纯净Debian 7

bash Network-Reinstall-System-Modify.sh -Debian_7
⑥. 一键网络重装纯净Ubuntu 18.04（推荐）

bash Network-Reinstall-System-Modify.sh -Ubuntu_18.04
⑦. 一键网络重装纯净Ubuntu 16.04

bash Network-Reinstall-System-Modify.sh -Ubuntu_16.04
⑧. 一键网络重装纯净Ubuntu 14.04

bash Network-Reinstall-System-Modify.sh -Ubuntu_14.04
【安装Windows系统】

*警告：你需要购买来自Microsoft或其合作伙伴正版系统授权并激活系统使用。继续安装即代表您知悉并已经购买正版授权。

①. 一键网络重装纯净Windows Server 2019（推荐）

bash Network-Reinstall-System-Modify.sh -Windows_Server_2019
②. 一键网络重装纯净Windows Server 2016

bash Network-Reinstall-System-Modify.sh -Windows_Server_2016
③. 一键网络重装纯净Windows Server 2012 R2

bash Network-Reinstall-System-Modify.sh -Windows_Server_2012R2
④. 一键网络重装纯净Windows Server 2008 R2

bash Network-Reinstall-System-Modify.sh -Windows_Server_2008R2
⑤. 一键网络重装纯净Windows 7

bash Network-Reinstall-System-Modify.sh -Windows_7_Vienna
⑥. 一键网络重装纯净Windows Server 2003

bash Network-Reinstall-System-Modify.sh -Windows_Server_2003
【安装DD系统】

*如果您不了解这意味着什么，请不要进行操作。%ULR%应该替换为您自己的映像地址。

bash Network-Reinstall-System-Modify.sh -DD "%URL%"
恭喜，你已经完成了系统重装，享受当下的美好
当您执行完上面的2行命令，你的服务器将开始网络重装纯净系统。在完成安装前，您将无法进行连接管理。

因硬件配置和网络环境不同，安装全程需要15-60分钟，请耐心等待。安装完成即可通过IP:22(Linux SSH)/IP:3389(Windows RDP)进行连接。
