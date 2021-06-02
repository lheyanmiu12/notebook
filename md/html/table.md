###table 认识表格
|属性|值/描述|
|:-:|:-:|
|with|固定值，百分百|
|height|高度 固定值 百分比|
|border|边框 固定值|
|align|对齐方式 left/right/center|
|cellspacing|单元格与单元格的间距(细胞间距)|
|cellpadding|文字与边框的距离|
|colspan|合并行|
|rowspan|合并列|
####快速写法
```
<!--table标签
4行3列的表格
table>tr*4>td*3
table>tr*4>td{单元格$}*3-->
```

   - 关于合并   
不管合并与否，一定要保证每一行的TD数量必须一致   
列的合并   
1.先找到要合并的最左边的单元格   
2.加colspan属性。值是被合并的单元格的个数   
3.把被合并的单元格删除或注释行的合并   
行的合并   
1.先找到要合并的最左边的单元格   
2.加rowspan属性。值是被合并的单元格的个数   
3.把被合并的单元格删除或注释行列的合并      
行列的合并   
1.先找到要合并的最左边的单元格   
2.加rowspan和colspan属性。值是被合并的单元格的个数   
3.把被合并的单元格删除或注释   
   - example
```
<!--练习：创建九宫格表格，单元格与单元格间的间距为0，内容与边框的间距为10-->
answer
<body>
		<table width="60%" height="300" border="1" cellpadding="10" cellspacing="0" align="center">
			<tr>
				<td>1</td>
				<td>2</td>
				<td>3</td>
			</tr>
			<tr>
				<td>1</td>
				<td>2</td>
				<td>3</td>
			</tr>
			<tr>
				<td>1</td>
				<td>2</td>
				<td>3</td>
			</tr>
		</table>
	</body>
```