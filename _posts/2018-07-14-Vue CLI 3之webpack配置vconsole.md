---
author: qixin
date: 2017-07-14
layout: post
title: Vue CLI 3之webpack配置vconsole
img: http://pblq6h54x.bkt.clouddn.com/post/img/vconsole.png
tags: [前端, Vue]
---

安装 ``vconsole-webpack-plugin``

``npm install vconsole-webpack-plugin --save-dev``

``vue.config.js`` 文件配置里增加以下插件配置：

    var vConsolePlugin = require('vconsole-webpack-plugin');

    const argv = require('yargs').describe('debug', 'debug 环境').argv;

    module.exports = {
      configureWebpack: {
        plugins: [
          new vConsolePlugin({enable: !!argv.debug})
        ]
        }
    }

``package.json`` 文件配置：

    "scripts": {
        "serve": "vue-cli-service serve",  
        "debug": "vue-cli-service serve --debug",
        "build": "vue-cli-service build",
        "lint": "vue-cli-service lint"
    }

``npm run debug``开启vconsole

![vconsole演示效果](http://pblq6h54x.bkt.clouddn.com/post/img/vconsole_demo.png)
