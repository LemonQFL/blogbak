---
title: ajax-2
date: 2019-05-15 17:04:08
tags:
 - ajax
---


# Ajax跨域

## 介绍

因为由于浏览器的`同源(域)策略`,禁止ajax从一个域名请求另外一个域名上的数据。

原因：同源策略是浏览器的一个安全机制，是为了保护本地数据不被ajax响应回来的数据污染，也就是ajax请求发送了，服务器响应了，但是无法被浏览器接收。

## 演示跨域

跨域测试:使用Ajax请求第三方天气接口数据

api接口地址: <http://www.weather.com.cn/data/sk/101010100.html>     

其中101010100是每个地区的代号

## 如何才算跨域

如一个普通的url地址如下:

<http://www.abc.com:80/index.html>  

我们可以把上面的url地址分为四个部分:

- 协议:http或https 

- 一级(顶级)域名如：abc.com   baidu.com   

- 二级域名:www.abc.com 、image.baidu.com  

- 端口号: http协议默认是80端口, https默认是443   

以上四个部分,ajax请求的时候只要有一个地方不一样都算做跨域请求。
