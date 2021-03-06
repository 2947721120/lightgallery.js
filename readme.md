# lightgallery.js

![travis](https://travis-ci.org/sachinchoolur/lightgallery.js.svg?branch=master)
![bower](https://img.shields.io/bower/v/lightgallery.js.svg)
![npm](https://img.shields.io/npm/v/lightgallery.js.svg)

全功能的JavaScript灯箱画廊。无依赖.

![lightgallery](https://raw.githubusercontent.com/sachinchoolur/lightgallery.js/gh-pages/lightgallery.png)

## 演示

* [lightgallery demo](https://sachinchoolur.github.io/lightgallery.js/)
* [Codepen demo](https://codepen.io/sachinchoolur/pen/qNyvGW)

## 主要特点

*充分响应。
*模块化结构与内置的插件。
*用于移动设备的触摸支持。
*鼠标拖动支持桌面。
*双击/双击可看到图像的实际大小。
*动画缩略图。
*社交媒体共享。
* YouTube上，Vimeo的，土豆网，VK和HTML5视频支持。
*20 +硬件加速CSS3过渡。
*动态模式。
*全屏幕的支持。
*支持变焦。
*浏览器历史记录的API。
*响应图像。
* HTML iframe支持。
*在一个页面上的多个实例。
*通过CSS（SCSS）和设置轻松定制。
*智能图像预加载和代码优化。
*键盘导航桌面。
*字体图标支持。
* 还有很多。

## 浏览器支持

lightgallery支持所有主要的浏览器IE9，包括以上.

## Installation

### 安装 Bower

You can install `lightgallery` using the [Bower](http://bower.io) package manager.

```sh
bower install lightgallery.js --save
```

### npm

您还可以找到 `lightgallery` on [npm](https://www.npmjs.com/).

```sh
npm install lightgallery.js
```

### 从GitHub下载

您也可以直接从GitHub下载lightgallery.

## 包括CSS和JavaScript文件

首先，加 lightgallery.css 在 `<head>`里面 该文件的.

```html
<head>
    <link rel="stylesheet" href="css/lightgallery.css">
</head>
```

Then include `lightgallery.min.js` 到文档中。
如果你想包括任何lightgallery插件后可以将其包含 `lightgallery.min.js`.

```html
<body>
    ...

    <script src="js/lightgallery.min.js"></script>

    <!-- lightgallery plugins -->
    <script src="js/lg-thumbnail.min.js"></script>
    <script src="js/lg-fullscreen.min.js"></script>
</body>
```

Lightgallery还支持AMD，CommonJS的和ES6模块。
当您使用AMD确保lightgallery.js之前lightgallery模块加载.

```js
require(['./lightgallery.js'], function() {
    require(["./lg-zoom.js", "./lg-thumbnail.js"], function(){
        lightGallery(document.getElementById('lightgallery'));
    });
});
```

## 标记

lightgallery不强迫你使用任何类型的标记。你可以使用任何你想要的标记。
但我建议你使用以下的标记.
[Here](https://sachinchoolur.github.io/lightgallery.js/demos/html-markup.html)
you can find the detailed examples of different kinds of markup.

```html
<div id="lightgallery">
    <a href="img/img1.jpg">
        <img src="img/thumb1.jpg">
    </a>
    <a href="img/img2.jpg">
        <img src="img/thumb2.jpg">
    </a>
    ...
</div>
```

## 调用插件

最后，你需要通过添加下面的代码以启动图库.

```js
<script>
    lightGallery(document.getElementById('lightgallery'));
</script>
```

## 支持lightgallery

如果你喜欢lightgallery请盯着库支持项目或 <a href="https://twitter.com/intent/tweet?original_referer=https%3A%2F%2Fabout.twitter.com%2Fresources%2Fbuttons&ref_src=twsrc%5Etfw&text=lightgallery%20-%20Full%20featured%20%23javascript%20lightbox%20gallery%2C%20No%20%23jQuery%20-%20http%3A%2F%2Fbit.ly%2F2amlfJe" target="_blank">tweet</a> about this project.

## 资源

* [API 参考](https://sachinchoolur.github.io/lightgallery.js/docs/api.html)
* [事件](https://sachinchoolur.github.io/lightgallery.js/docs/api.html#events)
* [方法](https://sachinchoolur.github.io/lightgallery.js/docs/api.html#methods)
* [数据属性](https://sachinchoolur.github.io/lightgallery.js/docs/api.html#attributes)
* [动态变量](https://sachinchoolur.github.io/lightgallery.js/docs/api.html#dynamic)
* [萨斯变量](https://sachinchoolur.github.io/lightgallery.js/docs/api.html#sass)
* [模 API](https://sachinchoolur.github.io/lightgallery.js/docs/plugin-api.html)

## 演示

* Thumbnails
  * [Gallery with animated thumbnails](https://sachinchoolur.github.io/lightgallery.js/demos/)
  * [Gallery without animated thumbnails](https://sachinchoolur.github.io/lightgallery.js/demos/#normal-thumb)
* YouTube, Vimeo Video Gallery
  * [YouTube, Vimeo Video Gallery](https://sachinchoolur.github.io/lightgallery.js/demos/videos.html)
  * [Video Gallery Without Poster](https://sachinchoolur.github.io/lightgallery.js/demos/videos.html#video-without-poster)
  * [Video Player Parameters](https://sachinchoolur.github.io/lightgallery.js/demos/videos.html#video-player-param)
  * [Automatically load thumbnails](https://sachinchoolur.github.io/lightgallery.js/demos/videos.html#auto-thumb)
* HTML5 Video Gallery
  * [HTML5 Video Gallery](https://sachinchoolur.github.io/lightgallery.js/demos/html5-videos.html)
  * [HTML5 video gallery with videojs](https://sachinchoolur.github.io/lightgallery.js/demos/html5-videos.html#video-without-poster)
* [Transitions](https://sachinchoolur.github.io/lightgallery.js/demos/transitions.html)
* [Dynamic](https://sachinchoolur.github.io/lightgallery.js/demos/dynamic.html)
* [Events](https://sachinchoolur.github.io/lightgallery.js/demos/events.html)
* [Methods](https://sachinchoolur.github.io/lightgallery.js/demos/methods.html)
* [Iframe. External websites, Google map etc.](https://sachinchoolur.github.io/lightgallery.js/demos/iframe.html)
* [Captions](https://sachinchoolur.github.io/lightgallery.js/demos/captions.html)
* Responsive images
  * [Responsive images](https://sachinchoolur.github.io/lightgallery.js/demos/responsive.html)
  * [Responsive images with HTML5 srcset](https://sachinchoolur.github.io/lightgallery.js/demos/responsive.html#srcset-demo)
* [Gallery with fixed size](https://sachinchoolur.github.io/lightgallery.js/demos/fixed-size.html)
* [HTML Markup](https://sachinchoolur.github.io/lightgallery.js/demos/html-markup.html)
* [Facebook comments](https://sachinchoolur.github.io/lightgallery.js/demos/comment-box.html)
* [Easing](https://sachinchoolur.github.io/lightgallery.js/demos/easing.html)
* [History/hash plugin](https://sachinchoolur.github.io/lightgallery.js/demos/hash.html)
* [Social media share](https://sachinchoolur.github.io/lightgallery.js/demos/share.html)

## 内置模块

1. 缩略图 - [GItHub](https://github.com/sachinchoolur/lg-thumbnail.js) - [Docs](https://sachinchoolur.github.io/lightgallery.js/docs/api.html#lg-thumbnial)
2. Autoplay - [GItHub](https://github.com/sachinchoolur/lg-autoplay.js) - [Docs](https://sachinchoolur.github.io/lightgallery.js/docs/api.html#lg-autoplay)
3. Video - [GItHub](https://github.com/sachinchoolur/lg-video.js) - [Docs](https://sachinchoolur.github.io/lightgallery.js/docs/api.html#lg-video)
4. Fullscreen - [GItHub](https://github.com/sachinchoolur/lg-fullscreen.js) - [Docs](https://sachinchoolur.github.io/lightgallery.js/docs/api.html#lg-fullscreen)
5. Pager - [GItHub](https://github.com/sachinchoolur/lg-pager.js) - [Docs](https://sachinchoolur.github.io/lightgallery.js/docs/api.html#lg-pager)
6. Zoom - [GItHub](https://github.com/sachinchoolur/lg-zoom.js) - [Docs](https://sachinchoolur.github.io/lightgallery.js/docs/api.html#lg-zoom)
7. Hash - [GItHub](https://github.com/sachinchoolur/lg-hash.js) - [Docs](https://sachinchoolur.github.io/lightgallery.js/docs/api.html#lg-hash)
8. Share - [GItHub](https://github.com/sachinchoolur/lg-share.js) - [Docs](https://sachinchoolur.github.io/lightgallery.js/docs/api.html#lg-share)

## 支持

Please use GitHub [issue tracker](https://github.com/sachinchoolur/lightgallery.js/issues/new) in the event that you have come across a bug or glitch. It would also be very helpful if you could add a jsFiddle, which would allow you to demonstrate the problem in question.

Please use [stackoverflow](https://stackoverflow.com/search?q=lightgallery) instead of GitHub issue tracker if you need any help with implementing lightgallery in your project or if you have any personal support requests.

Do you like lightgallery? You can support the project by staring the GitHub repository or [tweet](https://twitter.com/intent/tweet?original_referer=https%3A%2F%2Fabout.twitter.com%2Fresources%2Fbuttons&ref_src=twsrc%5Etfw&text=lightgallery%20-%20Full%20featured%20%23javascript%20lightbox%20gallery%2C%20No%20%23jQuery%20-%20http%3A%2F%2Fbit.ly%2F2amlfJe) about this project.

Follow me on Twitter [@sachinchoolur](https://twitter.com/sachinchoolur) for the latest news, updates about this project.

I am re-writing [lightslider](https://github.com/sachinchoolur/lightslider) too in pure JavaScript, It will be completely compatible with lightgallery. Watch the repository to get latest updates.
