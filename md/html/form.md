###form标签
####form    表单标签，可以理解为一张文件纸，上门可以输出任意问题和答案

|属性|对应值|
|:-:|:-:|
|action|接收地址，通常是应该是一个后台的程序处理地址，php、jsp、.net、nodejs，如果不填，则默认提交本页面。|
|name|表单的名字，主要用区分表单|
|target|表单提交的页面的打开方式，_self,_blank或者是具体的窗体名字（例如iframe的名字）|
|method|get<ba>轻量的请求方式，信息量比较小，安全要求不高(浏览产品页面，文章页面，访问一些咨询页面),信息是存在url地址栏后面，例如login.php?username=gdgf&pw=eeri这样的形式来传输信息<br>post<br>较重的请求方式，信息量比较大，安全要求相对较高(上传文件，上传文章，网站登陆，验证等)|
###使用method的好处
- 前后分离（更快，更好，更高，不背锅）
- 前端：版面制作、交互制作、数据或许、数据提交                   
- 后台：提供API

- Example
```
<!--<iframe src="" name="ifr"></iframe>-->
<form action="login.php" name="login" method="post">
	用户名:<input type="text" name="username"/><br />
	密码:<input type="password" name="pw"/><br />
	<input type="submit"/>
</form>
```

##搜索框
**search：**搜索框  主要增加了一个快速清除内容的功能
兼容性：IE10+以上浏览器

##电话号码输入框
|属性类型|描述|
|:-:|:-:|
|tel|主要通过搭配pattern属性来检验正确的电话号码|
|pattern|检验规则，通常用正则表达式来表示<br>汕头号码正则表达式  "8[0-9]{8}"|
|required|必填|
**兼容性：IE10+以上浏览器支持**
- Example
```
<input type="tel" pattern="1[0-9]{10}" required/>
```

##颜色色板（拾色器）
```
<input type="color" name="color" />
```

##日期
|属性|描述|
|:-:|:-:|
|datetime-local|可选年月日十分|
|date|可选年月日|
|month|可选年月|
|week|可选年月日和周几（移动端几乎不兼容）|
|time|可选时分|
**兼容性：PC端除了IE和Safari不支持**   
- Example
```
<input type="datetime-local" name="datetime-local"/><br />
<input type="date" name="name"/><br />
<input type="month" name="month"/><br />
<input type="week" name="week"/><br />
<input type="time" name="time"/><br />
```

##数字范围选择器
|属性|描述|
|:-:|:-:|
|range|数字范围选择器|
|min|最小值|
|max|最大值|
|value|当前默认值|
|step|每次改动的步伐大小|
**兼容性：IE10+兼容**
```
<input type="range" min="0" max="100" step="10" value="0"/>
```


