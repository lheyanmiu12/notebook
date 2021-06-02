###CSS的三种引入方式
####第一种引入方式

**行内引入**（只能控制当前元素）
注意：不推荐的写法，因为结构混乱，切不利于重用。
- Example
```
<div style="width: 500px;height: 500px;background-color: darkorange;">
我是一个饼
</div>
```
<br>
**第二种引入方式**（只能针对当前的HTML元素）
注意：该写法通常不推荐使用，因为只能控制当前页面，不能重用到其他页面上
- Example
```
<head>
	<meta charset="UTF-8">
	<title></title>
	<style type="text/css">
		div{
			border-radius: 50%;
		}
	</style>
</head>
```
<br>
**第三种引入方式**
页外引入（可以针对一个或多个HTML元素）
注意：是一个独立的CSS文件，注意语法的写法。可以有效地重用样式。
- Example
```
	<head>
		<meta charset="UTF-8">
		<title></title>
		<link rel="stylesheet" type="text/css" href="xxx/xxx.css" />
```
<br>
##三种引入方式的注意事项：
**1.就近原则，在选择器和属性相同的情况下，谁更接近目标元素，则谁的优先级越高（由上往下读）。<br>2.不同的引入方式之间，尽量不要出现重复属性的样式属性。<br>3.在真正的生产环境中，尽量的用页外引入方式来写样式，方便我们管理HTML文件和样式文件。**