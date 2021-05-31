<h3 align="center">CSS Note:</h3>
注释：/* xxxxx */

 - **样式选择器：**

1.当内联样式： （自个儿就地设置自个儿的）


2.置于head-style中，根据元素选择样式 


3.id标记运用样式  
为标有**特定 id** 的 HTML 元素**指定样式**。
元素中以 id 属性来设置 id （body里）, **CSS 中 id 选择器以**  **`#` 来定义。**
		

    <style>
        #para1
        {
        	text-align:center;
        	color:red;
        } 
    </style>
    </head>
    
    <body>
        <p id="para1">你好，世界！！！</p>
        <p>此段落不受样式的影响。</p>
    </body>
		
4.类class名选择样式
class 选择器用于描述一组元素的样式，c有别于 id 选择器，class 可以在**多个元素中使用**。

    <style>
        .center
        {
        	text-align:center;
        }
    </style>
    </head>
    
    <body>
        <h1 class="center">标题居中</h1>
        <p class="center">段落居中。</p> 
    </body>

5.元素. class名

    <style>
        p.center
        {
        	text-align:center;
        }
    </style>
    </head>
    
    <body>
        <h1 class="center">此标题不受影响</h1>
        <p class="center">此段落将居中对齐。</p> 
    </body>
**一个元素可以有多个class ,使用空格分隔：**

    <p class="xxx1 yyy2">XXSXXX</p>

***CSS优先级***
内联> id > class > 元素选择器

-   A 选择器都有一个权值，权值越大越优先；
-   B 当权值相等时，后出现的样式表优于先出现的；
-   C 网页编写者设置的 CSS 样式的优先权高于浏览器所设置的；
-   D 继承的 CSS 样式不如后指定的 CSS 样式；
-   E 在同一组属性设置中标**有 "!important" 规则的优先级最大；**  

<hr>

 - **Backgrounds背景：**

背景颜色：{background-color: #6495ed;}
 
背景图片：background-image: url('paper.gif');

背景平铺：background-repeat: repeat-x;

背景是否固定不随滚动移动：
background-attachment:fixed;

背景位置：
background-position:right top;
background-position:50% 50%;
background-position:50px 100px;

混合简写：

> body {
> background:#ffffff url('img_tree.png') no-repeat right top;
> }

顺序：color-image-repeat-attachment-position
<hr>

![盒子模型Box Model](https://7n.w3cschool.cn/statics/images/course/box-model.gif)

content（内容）就是盒子里装的东西，padding（内边距）就是怕盒子里装的东西损坏而添加的泡沫或者其他抗震防挤压的辅料，border（边框）就是盒子本身了，margin（外边距）则说明盒子摆放的时候不能全部堆在一起，要留一定空隙。

> content常指文字、图片等元素，但是也可以是小盒子（DIV嵌套）； padding只有宽度属性，可以理解为盒子中抗震辅料的厚度；
> border有大小和颜色之分，可理解为盒子的厚度以及这个盒子的颜色或材料； margin就是该盒子与其他东西要保留多大距离。
> 

**Position：**
`relative`和`absolute` 辨析：https://blog.csdn.net/weixin_42067967/article/details/80152403
在子元素内设置position:absolute。然后加top,left 之类。
因为absolute 的**绝对偏移**是相对与**已定位的**祖先元素，所以只要包裹它的元素是有position:relative，它就相对祖先元素定位，而这个距离在各浏览器上都一致。

***float element 相关:*** https://www.cnblogs.com/iyangyuan/archive/2013/03/27/2983813.html 

<hr>

**导航栏：**
`list-style-type:none` 移除列表前小标志。一个导航栏并不需要列表标记。
**块block导航栏：**
`display:block` - 显示块元素的链接，让整体变为可点击链接区域（不只是文本），它允许我们指定宽度
**水平导航栏**：
display:inline; 
<hr>
CSS 变量经常会定义在  :root  元素内，这样就可被所有选择器继承。

`:root`  是一个  pseudo-class  选择器匹配文档的根选择器，通常指  `html`  元素。

<hr>



> Written with [StackEdit](https://stackedit.io/).

<!--stackedit_data:
eyJoaXN0b3J5IjpbNTY4MjgyNzA4LDEwNzcwODMyODBdfQ==
-->