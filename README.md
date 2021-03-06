Auto-Refresh
============

Auto Refresh Chrome Extension。 

适用于前端开发的自动刷新chrome插件

# 自动刷新的chrome插件

## 功能

每次修改前端代码（JS CSS Html）后,只需要在编辑器Ctrl+S即可实时看到页面变化

1. Html和JS做修改后会自动刷新页面。
2. CSS的修改会以动画形式同步。
3. chrome插件支持跨域的ajax，远程的跨域文件也能实时更新。
4. 不需要按Ctrl+R来手动刷新了。

## 说明

![说明](http://gtms01.alicdn.com/tps/i1/T1TKlfFu4aXXbNKrY0-514-362.jpg)

* A: 点击“重新加载文件”，会重新加载页面上引用的js、css文件。
* B: 页面上所有的静态资源，只需要选中就可以添加到实时的监控中。
* C: 开关，开启or关闭监控。

## 原理

* 对选择监控的文件每秒发一次HTTP HEAD请求。
* 对比每次的请求回的Content-Type和Last-Modified。
* 如果HTTP头请求结果发生改变就自动刷新页面，不需要手动刷新了。
