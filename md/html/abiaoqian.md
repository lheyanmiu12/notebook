###a标签
####a标签

|属性|描述|
|:-:|:-:|
|herf|链接地址|
|title|鼠标悬停时的描述|
|alt|描述内容|
|target 页面打开的方式| _self自身打开      _blank新窗体打开|
|name|链接名字|
```
便捷跳转
<!--
	一键发邮件
	href="mailto:xxxxxxxx@xxxx.xxx"
-->
<a href="mailto:1026439166@qq.com">发邮件</a>

<!--
	一键拨打电话
	href="tel:xxxxxx"
-->
<a href="tel:13112165351">一键拨打</a>

<!--
	一键发送短信
	href="sms:xxxxxxxx"
-->
<a href="sms:13112165351">发送短信</a>
```
```
<!--http://开头的地址，称之为网络绝对地址-->
<a href="http://qq.com">我是一个网络地址</a>

<!--相对地址，引入方和被引入方之间的关系，称谓相对关系，根据这个关系，
可以写出相对地址，只要该相对关系不要改变，则路径一直生效。-->
<a href="2222.html">我是一个相对地址</a>
<a href="page/page1.html">点击跳转page1</a>
```

