###ul标签
####ul 无序列表
快速写法:
```
ul>li{新闻$}*3
```

|type类型|描述|
|:-:|:-:|
|circle|空心圆|
|disc|实心圆|
|square|方形|

- Example
```
<ul type="circle">
	<li>首页</li>
	<li>
		产品列表
		<ul type="disc">
			<li>夹克</li>
			<li>裤子</li>
			<li>秋装</li>
		</ul>
	</li>
	<li>新闻中心</li>
</ul>
```