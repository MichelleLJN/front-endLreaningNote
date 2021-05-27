<h4>Html 是网页的结构，CSS 是网页的样式，Javascript是行为。</h4>
注释：

    <!-- xxxxxx -->

 **- head**

 - `<head>`

元素包含了所有的头部标签元素。描述了文档的各种**属性和信息**，其中包括文档的标题、在 Web 中的位置以及和其他文档的关系等。在 `<head>`元素中你可以插入脚本（scripts）, 样式文件（CSS），及各种 meta 信息。

可以添加在头部区域的元素标签为:

     <title>, <style>, <meta>, <link>, <script>, <noscript> 和 <base>。
<hr>

 - `<base>`

 标签描述了基本的链接地址/链接目标，该标签作为 HTML 文档中*所有的链接* 规定**默认地址或默认目标**（target）:
   

     <head>
        <base href="//www.w3cschool.cn/images/" target="_blank">
        </head>

 - `<link>`

 标签定义了文档与外部资源之间的关系。
 常用于连接到**样式**css：

     <link rel="stylesheet" type="text/css" href="mystyle.css">

 - `<style>` 标签
样式详细，默认下，元素内**写入的样式**指令将**被认为是CSS**。=使用外部样式用`<link>`
 1. 在head里写：

		   <style type="text/css">
	        h1 {color: green;}
	        p{color: blue;}  
		    </style> 

 2. 在控件的标签里写

		<body style="background-color: red;">
		<p style="font-family:arial; color: green; font-size:20px;">This is a paragraph.</P>
		</body>
				
<hr>
 **- 图片链接**
ep：

    <p>创建图片链接:
    <a href="http://www.xxxxx.html">
    <img src="/course/smiley.gif" alt="HTML 教程">
    </a>
    </p>
    
    <p>无边框的图片链接:
    <a href="http://www.xxxx.html">
    <img border="0" src="/smiley.gif" alt="HTML 教程"></a>
    </p>

<hr>

 - **html链接的 书签跳转用法**

	      <p>
	        <a href="#C4">查看章节 4</a> //链接跳转指向id=c4 处
	        </p>
	    
	    <h4>章节 1</h4>
	    <p>这边显示该章节的内容……</p>
	    <h4>章节 2</h4>
	    <p>这边显示该章节的内容……</p>
	    <h4>章节 3</h4>
	    <p>这边显示该章节的内容……</p>
	    <h4><a id="C4">章节 4</a></h4> // 标记id=“C4”
	    <p>这边显示该章节的内容……</p>

<hr>

 - `<img>`标签：

		<img src="url" alt="some_text">

src显示图片**源**地址，可以是本地文件地址也可以是图片网页地址。
 alt则是在图片打不开的时候，**代替出现**的文字内容。

<hr>

 - **表格Table**
ep:
		

		<html>
			    	<head>
			    		<meta charset="utf-8">
			    		<title>This is the Title bar</title>
			    	</head>
			    	<body>
			    		<table border="2" width = "400" height = "150" 
			    bordercolor = "green" bgcolor = "yellow"> 
			    		// if背景为图片加：background = "/images/test.png"
			    			<caption>This is title of the table</caption> 
			    			// 表的标题
			    			<tr>   // tr表示一行
			    				<th>Header 1</th>   // 行表头
			    				<th>Header 2</th>	
			    			</tr>
			    			<tr>
			    				<<td>1st row, 1st cell </td>  //td 表示一列
			    				<td>1st row, 2 cell</td>
			    			</tr>
			    			<tr>
			    				<<td>2 row, 1st cell </td>
			    				<td>2 row, 2 cell</td>
			    			</tr>
			    		</table>
			    	</body>
			    </html>

<html>
	<head>
		<meta charset="utf-8">
		<title>This is the Title bar</title>
	</head>
	<body>
		<table border="2" width = "400" height = "150" 
		bordercolor = "green" bgcolor = "yellow">  <!-- if背景为图片加：background = "/images/test.png" -->
			<caption>This is title of the table</caption>
			<tr>
				<th>Header 1</th>
				<th>Header 2</th>	
			</tr>
			<tr>
				<<td>1st row, 1st cell </td>
				<td>1st row, 2 cell</td>
			</tr>
			<tr>
				<<td>2 row, 1st cell </td>
				<td>2 row, 2 cell</td>
			</tr>
		</table>
	</body>
</html>

<hr>

 - **列表List**
有序列表 ol li
无序列表 ul li
定义列表 dl dt dd （dd是dt的低一级别，自动缩进）

	    <div> 定义文档区块，块级(block-level)

	    <span> 定义 span，用来组合文档中的行内元素。
<hr>

 - **部分字符**
空格：`&nbsp; &#160;`

<小于：`&lt; &#60;`

》大于： `&gt; &#62;`

”单引号：`&quot; &#34;`

&和号：`&amp;&#38;`

<hr>

 - **表单：**

是一个包含表单元素input element的区域。

表单使用表单标签 <form> 来设置:

    <form>
    .
    input elements
    .
    </form>
最常用的form element：

 - input element输入元素:

	    <input type="#" name="xxx">
几种常用type：
1. 文本框。 type=“text”  
 `<input type="text" name="userName">`
		（*placeholder属性可显示文本域中默认文本）

	    <from action="#">  
	    <!--action属性的值指定了表单提交到服务器的地址。-->
    		用户名<input type="text" placeholder="username"/>
    	</from>

2. 密码。 type="password"

	    <form>
	    密码: <input type="password" name="pwd">
	    </form>
3. 单选按钮radio button。 type="radio"
		
	    <form>
    		<input type="radio" name="sex" value="male">男<br>
    		<input type="radio" name="sex" value="female">女
    	</form>
***name**是控件的**名称**（多个控件可以取同一个名称），**value**是控件的**值***

> name相当于是一个变量名，value相当于是一个变量的值，在JS中以及向网站后端传送参数时，与value一起用，比如name是“color”，value是“red”，那么就会有参数color=“red”。
> id是用来唯一标识一个容器，在CSS样式表和JS中都可能会用到，用来调节被id标识的容器的样式和动态效果
> 
4.多选框。type="checkbox"

    <form>
    <input type="checkbox" name="vehicle" value="Bike">我有自行车<br>
    <input type="checkbox" name="vehicle" value="Car">我有小车
    </form> 
5.提交按钮。type="submit"

    <form name="input" action="html_form_action.php" method="get">
    Username: <input type="text" name="user">
    <input type="submit" value="Submit">
    </form>

> Written with [StackEdit](https://stackedit.io/).


<!--stackedit_data:
eyJoaXN0b3J5IjpbMTE5OTM1OTQ5NF19
-->