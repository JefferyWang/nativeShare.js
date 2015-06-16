nativeShare
======

nativeShare是一个可以通过javascript直接调用原生分享的工具.  [demo](http://blog.wangjunfeng.com/demo/native_share/)

我们知道现在我们无法直接通过js直接跳转到微信和QQ等软件进行分享,但是现在像UC浏览器和QQ浏览器这样的主流浏览器自带一个分享工具,而他们也有自己定义的js接口.我们通过调用浏览器的接口去调用浏览器的分享,从而实现原生分享功能.是不是很酷呢?

该工具具有以下特点:

* 支持原生微博、微信好友、微信朋友圈、QQ好友、QQ空间分享

* 支持调用浏览器更多分享功能

* 注意:目前仅支持手机UC浏览器和QQ浏览器

github项目地址:  [https://github.com/JefferyWang/nativeShare.js](https://github.com/JefferyWang/nativeShare.js)

Git@OSC项目地址:  [http://git.oschina.net/wangjunfeng/nativeShare.js](http://git.oschina.net/wangjunfeng/nativeShare.js)

扫描二维码访问Demo
--------------------

![Demo](http://qrapi.cli.im/qr?data=http%253A%252F%252Fblog.wangjunfeng.com%252Fdemo%252Fnative_share%252F&level=H&transparent=false&bgcolor=%23ffffff&forecolor=%23000000&blockpixel=12&marginblock=1&logourl=&size=280&kid=cliim&key=95f6dfd09d364c85a17da72a307b24c5)

使用方法
--------------------

* 引入CSS文件

``` html
<link rel="stylesheet" href="nativeShare.css"/>
```

* 在需要放分享的地方插入以下代码

``` html
<div id="nativeShare"></div>
```

* 添加配置,并实例化

``` javascript
<script>
    var config = {
        url:'http://blog.wangjunfeng.com',// 分享的网页链接
        title:'王俊锋的个人博客',// 标题
        desc:'王俊锋的个人博客',// 描述
        img:'http://www.wangjunfeng.com/img/face.jpg',// 图片
        img_title:'王俊锋的个人博客',// 图片标题
        from:'王俊锋的博客' // 来源
    };
    var share_obj = new nativeShare('nativeShare',config);
</script>
```

截图
--------------------

![分享列表](http://i1.tietuku.com/5e6c8ab36cfb7990.jpg)
![微博分享](http://i1.tietuku.com/b95968a5a28720a4.jpg)
![朋友圈分享](http://i1.tietuku.com/933063f83bffe114.jpg)
![微信好友分享](http://i4.tietuku.com/0605788e4c9dd17d.jpg)
![QQ好友分享](http://i1.tietuku.com/cde46bc93b8677fa.png)
![QQ空间分享](http://i1.tietuku.com/5fa7f7dc87d4215f.png)
![更多](http://i1.tietuku.com/9f391d6e086aecad.jpg)
