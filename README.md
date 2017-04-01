#### 郑重声明 ####

*	－软件仅供科研、学习、教育等一切合法目的使用，严禁一切违法行为
*	－由于采用的是VPN技术，所有的网络通信都有可能被截获，涉及个人财产安全的操作请绕行

#### 欢迎使用 UVPN 科学上网神器 ####

一直以来，我们都可以修改电脑上的hosts文件实现科学上网，而在Android系统中，hosts文件保存在system分区中，在没有root的情况下，是无法修改的。本软件的存在，使得你可以“修改”hosts文件，实现科学上网。

##### 特点如下 #####

*	－可以随时导入、导出hosts文件，实现科学上网
*	－可以对本软件中的hosts文件进行导入、导出的操作
*	－内建DNS服务器，并且可以配置上游DNS服务器
*	－使用shadowsocks ss-server/ss-local软件，可以配置连接shadowsocks远程服务器
*	－包含流量流计，数据来自ss-server服务，但要注意统计只包含TCP连接相关的数据
*	－由于使用本软件会创建VPN连接，而Android系统同一时刻只能有VPN连接，VPN连接数量受限
*	－包含DNS服务器、ss-server服务、ss-local服务、VPN服务、udpgw服务，各模块可以独立运行

##### 注意事项 #####

*	－DNS服务器会占用本机的5353端口，用于接收DNS请求报文
*	－shadowsocks – ss-server会占用本机的8443端口，用来与ss-local进行socket通信
*	－shadowsocks – ss-local（socks5 server)会占用本机的1080端口，用来与badvpn - tun2socks进行socket通信
*	－badvpn – udpgw会占用本机的8700端口，用来与badvpn - tun2socks进行socket通信
*	－Android 6.0开始支持Always-on VPN, 本软件暂时不支持这个功能，请不要打开这个选项

##### 项目主页 #####

*	https://github.com/phope2000/android-apk-uvpn
*	Copyright (C) 2017 phope2000@gmail.com

#### 关于hosts文件 ####

本软件没有内置hosts文件，请自行从网上下载

#### 相关软件信息 ####

本软件所使用的开源软件如下：

*	1. badvpn

	源码：https://github.com/ambrop72/badvpn

	版权：BSD https://github.com/ambrop72/badvpn#license

*	2. dnsmasq

	官网：http://www.thekelleys.org.uk/dnsmasq/doc.html

	源码：https://android.googlesource.com/platform/external/dnsmasq/

	版权：https://android.googlesource.com/platform/external/dnsmasq/+/android-6.0.1_r65/NOTICE

*	3. libancilary

	官网：http://www.normalesup.org/~george/comp/libancillary/

	源码：https://github.com/shadowsocks/libancillary/

*	4. libev

	官网：http://software.schmorp.de/pkg/libev

	源码：https://github.com/shadowsocks/libev

*	5. libevent

	官网：http://libevent.org/

	源码：https://github.com/libevent/libevent

	版权：BSD

*	6. libsodium

	官网：https://libsodium.org

	源码：https://github.com/jedisct1/libsodium

	版权：https://github.com/jedisct1/libsodium/blob/master/LICENSE

*	7. libudns

	官网：http://www.corpit.ru/mjt/udns.html

	源码：https://github.com/shadowsocks/libudns

	版权：LGPL

*	8. mbedtls

	官网：https://tls.mbed.org/

	源码：https://github.com/ARMmbed/mbedtls

	版权：APACHE 2.0

*	9. pcre

	源码：https://android.googlesource.com/platform/external/pcre/+/android-7.1.1_r23

	版权：https://android.googlesource.com/platform/external/pcre/+/android-7.1.1_r23/NOTICE

*	10. shadowssocks-libev

	官网：https://shadowsocks.org/

	源码：https://github.com/shadowsocks/shadowsocks-libev

*	11. libloom

	官网：https://github.com/jvirkki/libbloom

	源码：https://github.com/shadowsocks/libbloom

	版权：BSD

*	12. libcork

	官网：http://libcork.readthedocs.org/

	源码：https://github.com/shadowsocks/libcork

	版权：https://github.com/redjack/libcork/blob/develop/COPYING

*	13. libipset

	官网：https://github.com/redjack/ipset

	源码：https://github.com/shadowsocks/ipset

	版权：https://github.com/redjack/ipset/blob/develop/LICENSE.txt

#### 写在最后 ####

感谢各位大神！
