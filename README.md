# 《一台普通电脑的 NAS 之旅 》

本项目将指导你从零开始构建一台家庭 NAS 网络存储服务器，从硬件到系统再到程序，完全自己动手搞定。

## 构建目标

遵照本项目的指导，你最终会将一台普通的计算机（PC）打造成为具有以下功能的 NAS 服务器：

* 多用户私有网盘
* HTTP、BT 全能下载机
* 局域网文件共享
* 跨平台文件同步
* Apple TimeMachine

搭配云服务器、国际域名、邮件推送等云计算资源，将能实现以下功能：

* 通过互联网访问网盘等功能
* 远程管理服务器
* 离线下载
* 基于 P2P 的虚拟专用网
* E-mail 故障通知

## 适用群体

原则上本方案适用于任何人，我们会尽可能提供详细的操作说明，没有 Linux 系统使用经验的用户可能需要额外掌握一些知识，因此构建过程会相应延长。

## 项目状态

本项目内容正在进行创作，在此期间，目录、标题和内容随时都可能发生较大变动。建议 **暂时** 不要采用本项目指南构建用于生产环境的 NAS 服务器。

## 目录

* [项目概述](summary.md)
* [准备工作](preparations.md)
* [制作 U 盘系统安装盘](system-installation/usb-installer.md)
* [安装 Debian 操作系统](system-installation/system-installation.md)
* [第一次启动](the-first-boot/the-first-boot.md)
* [更新系统](initialization/system-upgrade.md)
* [通过 SSH 远程管理服务器](initialization/use-ssh.md)
* [存储管理](storage)
	* [准备数据盘](storage/prepare-hdd.md)
   * [系统 U 盘分区容量调整](storage/resize-flashdrive.md)
	* [方案一 直接使用硬盘分区](storage/case-one.md)
	* [方案二 硬盘 + LVM](storage/case-two.md)
	* [方案三 直接使用 RAID 磁盘阵列](storage/case-three.md)
	* [方案四 RAID + LVM](storage/case-four.md)
* [Samba 文件共享](samba.md)
* [常见问题](questions)
	* [UEFI 模式 Debian 启动失败进入 initramfs](questions/uefi-cannot-boot.md)

## 采用的开源项目

* [Debian](https://www.debian.org/)
* [NextCloud](https://www.nextcloud.com)
* [Syncthing](https://syncthing.net/)
* [Aria2](https://aria2.github.io/)
* [qBittorrent](https://www.qbittorrent.org/)
* [Samba](https://www.samba.org/)
* [Apache](http://httpd.apache.org/)
* [MariaDB](https://downloads.mariadb.org/)
* [Tinc](https://www.tinc-vpn.org/)
* [Netatalk](http://netatalk.sourceforge.net/)
* [Avahi](http://avahi.org/)
* [frp](https://github.com/fatedier/frp)
* [webui-aria2](https://github.com/ziahamza/webui-aria2)

## 写作规范
[GetNAS 项目写作规范](writing-guidelines.md)

## 赞助 & 合作

* [赞助 GetNAS 项目](sponsor/sponsor.md)

## 版权 & 许可

版权所有 ©️ 2017 [于鸿儒](https://twitter.com/herald_yu) (Herald Yu)

[<img alt="知识共享许可协议" style="border-width:0" src="images/by-nc-nd-88x31.png">](http://creativecommons.org/licenses/by-nc-nd/4.0/deed.zh)

本作品采用 [署名-非商业性使用-禁止演绎 4.0 国际许可协议](http://creativecommons.org/licenses/by-nc-nd/4.0/deed.zh) 进行许可。
