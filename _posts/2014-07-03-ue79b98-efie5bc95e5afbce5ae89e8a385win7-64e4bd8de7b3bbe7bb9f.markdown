---
author: QX4546
comments: true
date: 2014-07-03 11:02:19+00:00
layout: post
link: http://xinchyi.com/archives/302
slug: u%e7%9b%98-efi%e5%bc%95%e5%af%bc%e5%ae%89%e8%a3%85win7-64%e4%bd%8d%e7%b3%bb%e7%bb%9f
title: U盘 EFI引导安装win7 64位系统
wordpress_id: 302
categories:
- 电脑相关
tags:
- win7
- windows
---

前两天朋友找我装系统，普通U盘安装时出现“windows无法安装到这个磁盘。选中的磁盘采用GPT分区形式”，无奈只能用EFI引导安装，刚好以前接触过UEFI，所以安装过程也没遇到什么问题。下面将安装步骤记录如下：

**首先，将系统镜像、EFI x64文件（红色圈中）解压缩到U盘根目录，注意U盘格式为FAT32。**

[![efi-1](http://xinchyi.com/wp-content/uploads/2014/07/efi-1-300x238.jpg)](http://xinchyi.com/wp-content/uploads/2014/07/efi-1.jpg)

**进入BIOS，从EFI启动（白色部分回车）**

[![efi-2](http://xinchyi.com/wp-content/uploads/2014/07/efi-2-300x200.jpg)](http://xinchyi.com/wp-content/uploads/2014/07/efi-2.jpg)

**回车后会进入下面这个页面**

[![efi-3](http://xinchyi.com/wp-content/uploads/2014/07/efi-3-300x203.jpg)](http://xinchyi.com/wp-content/uploads/2014/07/efi-3.jpg)

**找到启动U盘，输入命令fs1: ,当然不一定是fs1,视具体情况而定**

[![efi-4](http://xinchyi.com/wp-content/uploads/2014/07/efi-4-300x203.jpg)](http://xinchyi.com/wp-content/uploads/2014/07/efi-4.jpg)

**进一步输入命令ls可以查看内部包含文件，可以看到BOOTMGFW.EFI文件，进一步输入命令BOOTMGFW.EFI进入安装界面，后面跟普通安装一样，在此不做过多赘述**

[![efi-5](http://xinchyi.com/wp-content/uploads/2014/07/efi-5-300x203.jpg)](http://xinchyi.com/wp-content/uploads/2014/07/efi-5.jpg)
