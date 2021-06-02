###base 统一化路径标签
base 统一化路径标签   
href 具体的参照物地址   
注意：协商这个base标签的页面，所有的链接，都会从该参照物地址开始算起，   所以要注意资源和页面链接的写法
####Example
```
<html>
	<head>
		<meta charset="UTF-8">
		<title></title>
		<base href="/20171207HTML/1/2/3/4/5/"/>
	</head>
	<body>
		<a href="index.html">我要去访问一个文件目录很深的文件</a>
	</body>
</html>
```
```
<html>
	<head>
		<meta charset="UTF-8">
		<title></title>
		<base href="/20171207HTML/" />
	</head>
	<body>
		我是你要找的人
		<a href="统一化路径base标签.html">返回起点</a>
	</body>
</html>
```
