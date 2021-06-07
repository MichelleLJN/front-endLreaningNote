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
    
[enter link description here](https://atts.w3cschool.cn/attachments/image/20201112/1605147193236568.png)

表单验证：
1、valueMissing

目的：确保表单控件中的值已填写。
用法：在表单控件中将required特性设置为true。
示例：
```
<input type="text" name="myText" required>

```

详细说明：如果表单控件**设置了required特性**，那么在用户填写或者通过代码调用方式填值之前，控件会一直处于无效状态。例如，空的文本输入框无法通过必填检查，除非在其中输入任意文本。输入值为空时，valueMissing会返回true。

2、typeMismatch

目的：保证控件值与预期类型相匹配(如numbe、email、URL等).

用法：指定表单控件的type特性值。

示例：

```
<input type="email" name="myEmail">

```

详细说明：特殊的表单控件类型不只是用来定制手机键盘， 如果浏览器能够识别出来表单控件中的输入不符合对应的类型规则，比如email地址中没有@符号，或者number型控件的输入值不是有效的数字，那么浏览器就会把这个控件标记出来以提示类型不匹配。无论哪种出错情况，typeMismatch将返回true。

3、patternMismatch

目的：根据表单控件上设置的格式规则验证输入是否为有效格式。

用法：在表单控件上设置pattern特性，井赋予适当的匹配规则。

示例：

```
<input type="text" name="creditcardnumber" pattern="[0-9]{16}" title="A credit
card number is 16 digits with no spaces or dashes">

```

详细说明：pattern特性向开发人员提供了一种强大而灵活的方式来为表单的控件值设定正则表达式验证机制。当为控件设置了pattern特性 后，只要输入控件的值不符合模式规则，patternMismatch就会返回true值。从引导用户和技术参考两方面考虑，你应该在包含pattern特性的表 单控件中设置title特性以说明规则的作用。

4、tooLong

目的：避免输入值包含过多字符。

用法：在表单控件上设置maxLength特性。

示例：

```
<input type="text" name="limitedText" maxLength="140">

```

详细说明：如果输入值的长度超过**maxLength**， tooLong特性会返回true。虽然表单控件通常会在用户输入时，限制最大长度，但在有些情况下，如通过程序设置，还是会超出最大值。

5、rangeUnderflow

目的：限制**数值型控件的最小值**。

用法：为表单控件设置min特性，并赋予允许的最小值。

示例：

```
<input type="range" name="ageCheck" min="18">

```

详细说明：在需要做数值范围检查的表单控件中，数值很可能会暂时低于设置的下限。此时，ValidityState的rangeUnderflow特性将返回true。

6、rangeOverflow

目的：限制**数值型控件的最大值**。

用法：为表单控件设置max特性，并赋予允许的最大值。

示例：

```
<input type="range" name="kidAgeCheck" max="12">

```

详细说明：与rangeUnderflow类似，如果一个表单控件的值比max更大，特性将返回true。

7、stepMismatch

目的：确保输入值符合min、max及step即设置。

用法：为表单控件设置step特性，指定数值的增量。

示例：

```
<input type="range" name="confidenceLevel" min="0" max="100" step="5">

```

详细说明：此约束条件用来保证数值符合min、max和step的要求。换句话说，当前值必须是最小值与step特性值的倍数之和。例如，范围从0到100，step特性值为5，此时就不允许出现17，否则stepMismatch返回true值。

8、customError

目的：处理应用代码明确设置及计算产生的错误。

用法：调用setCustomValidity(message)将表单控件置于customError状态。

示例：

```
passwordConfirmationField.setCustomValidity("Password values do not match.");

```

详细说明：浏览器内置的验证机制不适用时，需要显示自定义验证错误信息。当输入值不符合语义规则时，应用程序代码应设置这些自定义验证消息。

自定义验证消息的典型用例是验证控件中的值是否一致。例如，密码和密码确认两个输人框的值不匹配。只要定制了验证消息，控件就会处于无效状态，并且customError返回true。要清除错误，只需在控件上调用setCustomValidity("")即可。
> Written with [StackEdit](https://stackedit.io/).


<!--stackedit_data:
eyJoaXN0b3J5IjpbMTgxMTY5MTk0M119
-->