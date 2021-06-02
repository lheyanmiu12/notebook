##area热区标签
####href与src区别   
href 从页面跳到外部页面   
src  把外部资源引到本页面

|shape属性|形状描述|
|:-:|:-:|
|rect|矩形|
|circlr|圆形|
|poly|多边形|
####Example
```
<img src="img/xxx.jpg" alt="" usemap="#hotmap" />
<map name="hotmap">
	<area shape="rect" coords="x,x,x,x" href="跳转地址.html" />
	<area shape="circle" coords="x,x,x" href="跳转地址.html" />
	<area shape="poly" coords="x,x,x,x,x,x" href="跳转地址.html" />
</map>
<img src="img/map.jpg" alt="" usemap="#hotmap" />
<map name="hotmap">
	<area shape="rect" coords="182,122,280,204" href="img标签.html" />
	<area shape="rect" coords="420,213,525,341" href="img/3.jpg" />
	<area shape="circle" coords="637,88,60" href="a标签.html" />
	<area shape="poly" coords="350,13,411,93,287,93" href="" />
</map>
```


