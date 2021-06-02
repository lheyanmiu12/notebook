###class与id选择器
**class与id选择器：css提供由用户自定义标签名称的选择符，用户可以用class和id选择符<br>来对页面中的xhtml标签进行自定义名称，从而达到拓展xhtml标签以及html标签的组合**
####class选择器
```
以class属性所对应的名字作为目标的名字，记得前面加个“.”符号。
注意：可以用class来代替id选择器，并且class选择器还可以多次重用，可以更好的控制一个或多个标签。
```

- Example
```
<head>
<style type="text/css">
.bg_black{
		background:black;
	}
</style>
</head>
<body>
	<p class="bg_black">
		今天是周一，天气不错，起床困难。
	</p>
	<p id="p2">
		我是p2
	</p>
	
	<p class="bg_black">
		我是p3
	</p>
</body>
```

####id选择器
```
以id的名字作为目标名，记得前面要加一个#符号。
 注意：一个页面只能存在一个唯一的ID。并不推荐使用，因为后期JS要常用到ID这个属性，可能会有冲突。
```
####写法示例：
```
<style type="text/css">
#p2{
	color: pink;
}
```