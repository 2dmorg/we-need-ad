we-need-ad
==========

我们站长需要广告！因为广告是我们唯一的收入来源。
但是现在一些无素质网站真的是广告满天飞，不堪忍受，令用户不得不使用广告屏蔽插件，而这样一来其他正常的广告，尤其那些站长精心设计的广告位置和内容，都被屏蔽了，所以，我们这些善良有素质的站长需要一个工具来提示用户，“请您将本站添加进您广告屏蔽插件的白名单”，于是，就有就有了这款工具。

由于本人刚入门js，简直就是菜鸟，如果有建议请不吝赐教～～

很简单，在head中引用
```python
<script src="你的目录/ad.js"></script>
```
ad.js这个文件里面内容
```python
document.write('<div id="ad">这里放你的广告内容</div>') /*在这个div里放你的广告，你可以把你原先的广告div放到这里来*/
```
在您网页的</head>标签前插入
```python
<script type="text/javascript">
    if (document.getElementById("ad") == undefined){
       document.write('<p>亲～您为嘛要使用广告屏蔽插件呢。本站压根儿没广告啊？其它网站里正常广告还是不要屏蔽了，人家指着广告吃饭呢，哪个网站广告实在多得忍不了，再添加进屏蔽名单好了——————<strong>2分米</strong></p>');
       }
</script>
```
然后就OK了。    