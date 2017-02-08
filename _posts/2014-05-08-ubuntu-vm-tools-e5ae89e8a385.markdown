---
author: QX4546
comments: true
date: 2014-05-08 16:32:07+00:00
layout: post
link: http://xinchyi.com/archives/167
slug: ubuntu-vm-tools-%e5%ae%89%e8%a3%85
title: Ubuntu vm-tools 安装
wordpress_id: 167
categories:
- 电脑相关
tags:
- linux
- ubuntu
- 虚拟机
---

探究Android，用到了虚拟机，顺便拾起一些Linux基础知识。Ubuntu vm-tools 安装，比较简单，没什么技术含量，首先是简单的Linux命令行（红色部分），出现yes的地方输入y，剩下一路回车。

xinchyi@xinchyi-virtual-machine:~$ cd /tmp
xinchyi@xinchyi-virtual-machine:/tmp$ cd ./vmware-tools-distrib
xinchyi@xinchyi-virtual-machine:/tmp/vmware-tools-distrib$ sudo ./vmware-install.pl
[sudo] password for xinchyi:
A previous installation of VMware Tools has been detected.

The previous installation was made by the tar installer (version 4).

Keeping the tar4 installer database format.

You have a version of VMware Tools installed. Continuing this install will
first uninstall the currently installed version. Do you wish to continue?
(yes/no) [yes] y

Uninstalling the tar installation of VMware Tools.

Stopping services for vmware-tools

initctl: Unknown instance:
Stopping services for vmware-tools-thinprint

initctl: Unknown instance:
File /etc/pulse/default.pa is backed up to /etc/pulse/default.pa.old.0.

update-initramfs: Generating /boot/initrd.img-3.13.0-24-generic
The removal of VMware Tools 9.6.2 build-1688356 for Linux completed
successfully.

......
