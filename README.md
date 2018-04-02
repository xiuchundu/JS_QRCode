
## (一)QRCode.js简介

QRCode.js 是一个用于生成二维码图片的插件。github地址为[https://github.com/davidshimjs/qrcodejs/](https://github.com/davidshimjs/qrcodejs/)

**在线实例**
[http://duchunxiu.cn/JS_QRCode/](http://duchunxiu.cn/JS_QRCode)

[http://www.shouce.ren/study/api/s/7020](http://www.shouce.ren/study/api/s/7020 "实例预览")

[http://www.shouce.ren/study/api/s/7021](http://www.shouce.ren/study/api/s/7021 "实例预览 ")


## 参数说明
```js
    new QRCode(element, option)
```
![](https://i.imgur.com/iV4Ql2f.jpg)

![](https://i.imgur.com/GxAvAwq.jpg)

[http://www.shouce.ren/api/d/id/11159](http://www.shouce.ren/api/d/id/11159 "下载")

## (二)qrcode.js生成二维码原理


qrcode.js在用于生成二维码的容器#qrcode内生成一个canvas标签和一个img标签，并且以base64的编码格式描述图片信息。

## 点击按钮，生成的二维码图片保存到本地
## 实现原理

将base64编码格式的图片转换成canvas画布
利用toDataUrl()方法将canvas画布信息转化为可供下载的url信息 toDataUrl()
构建下载链接并模拟点击，将图片下载到本机

## 基于qrcode.js案例demo实现将生成的二维码保存为本地图片

(1)构建一个用于下载的空的a标签

(2)将base64图片构建成画布并模拟点击a标签下载
