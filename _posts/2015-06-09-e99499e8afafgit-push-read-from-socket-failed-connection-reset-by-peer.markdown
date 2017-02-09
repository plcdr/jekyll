---
author: QX4546
comments: true
date: 2015-06-09 03:08:50+00:00
layout: post
title: git push ... reset by peer
categories:
- 电脑相关
tags:
- GIT
---

今天在git push 项目的时候，出现了错误：


    Read from socket failed: Connection reset by peer  
    fetal :could not read from remote repository


重新更换了SSH key不起作用，用ssh -T git@github.com测试可以连通。尝试了网上的N种方法，在希望渺茫的时候，天降神命令（谁用谁知道）：


    git config remote.origin.url git@github.com:your_username/your_project.git
