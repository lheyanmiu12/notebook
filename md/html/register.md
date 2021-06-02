###注册页面

**input：多功能的标签，可以根据type值进行对应功能的切换**

|属性类型|描述|
|:-:|:-:|
|type|类型属性，决定了这个input的功能，如果没有设置或设置了不合法的值，则全部默认为text（单行输入框）|
|name|该数据所对应的名字，主要是后台获取数据是使用|
|value|该数据所对应的值，如果不填则默认为空|
|maxlenght|该数据的值所允许的最大字符长度|
|disabled|禁止输入和禁止提交该数据|
|readonly|只读，禁止输入，但允许提交|
|size|控制输入框的显示长度|
|placeholder|提示语|

```
用户名：<input type="text" value="今天你学习了么？" maxlength="5" placeholder="请输入用户名"/>
```
<br>
**hidden：隐藏域，专门用来隐藏一些不需要用户操作的信息**
**注意：处理隐身，其余跟text没区别。**
```
密码：<input type="password" name="pw" placeholder="请输入密码"/><br />
ip: <input type="hidden" name="ip_address" value="192.168.1.1"/>
```

##radio单选框

|属性|描述|
|:-:|:-:|
|checked|表示选中的状态（单选框只允许设置其中一个为checked）|
|name|需要保证多个单选选项的名字是一样的|
|label标签|让自身内容和指定标签进行关联|
|for|关联属性  填写被关联的标签的ID|
- Example
```
性别:<label for="man">男</label>
    <input type="radio" name="sex"/ value="1" checke id="man">
 / 
    <label for="lady">女</label>
    <input type="radio" name="sex"/ value="2" id="lady">
```

##checkbox复选框
**此处name属性虽然名字可以不一样，但因为表示的是同一个数据，所以建议要用相同的名字，并且是一个数组（例如"movies[]"）,方便后台获取多组数据。**
- Example
```
钢铁侠<input type="checkbox" name="movies[]" value="1"/>|
蜘蛛侠<input type="checkbox" name="movie[]" value="2"/>|
复仇者联盟<input type="checkbox" name="movie[]" value="3"/>
X战警<input type="checkbox" name="movie[]" value="4"/>
```

##select下拉框
** 默认是单选模式<br>注意：<br>select和option是固定的组合，缺一不可。<br>multiple:加上该属性，则变为多选模式。**
```
所在城市：
<select name="city" multiple>
	<optgroup label="广东省">
		<option value="1">广州</option>
		<option value="2">深圳</option>
		<option value="3">清远</option>
		<option value="4">茂名</option>
		<option value="5">汕头</option>
		<option value="6">汕尾</option>
		<option value="7">揭阳</option>
	</optgroup>
	<optgroup label="其他省">
		<option value="8">北京</option>
		<option value="9">杭州</option>
		<option value="10">上海</option>
	</optgroup>
</select>
```

##上传文件
###注意事项:如果涉及到文件的上传，需要用post方式，并且form的enctype属性，要设置为multipart/form-data**

|属性类型|描述|
|:-:|:-:|
|capture|可以设置打开的程序 （针对移动端），camera、camcorder、microphone|
|accept|限制上传的文件类型     image/*  video/*  audio/*多种类型可以用都好隔开|
```
头像：<input type="file" name="headerurl[]" multiple capture="camera" accept="image/*","video/*"/>
```

##textarea文本域
**注意：没有value属性，它的值是直接写在标签对中间**<br>
**cols 列数<br>rows 行数**
```
自我介绍: 
			<textarea name="description" cols="100" rows="10" placeholder="请输入您的反馈或建议！" ></textarea>
```

##按钮
|属性类型|描述|
|:-:|:-:|
|reset|重置按钮，把表单还原为最初的状态|
|value|控制按钮的文字显示|
|image|图片提交按钮	其实就是用图片自定义了一个按钮而已|
|src|图片的源地址|

```
<input type="reset" value="重新跳伞！"/>
<input type="image" src="img/submit.jpg" style="width: 100px;"/>
<input type="submit" value="努力地发射把！"/>
```
