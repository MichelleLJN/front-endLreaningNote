
注释： //  单行； /* xxxxx */ 块注释
换行：\n
回车：\r 
Tab: \t

addEvenlistener:
事件传递有两种方式：**冒泡与捕获**。

事件传递定义了元素事件触发的顺序。 如果你将 <p> 元素插入到 <div> 元素中，用户点击 <p> 元素, 哪个元素的 "click" 事件先被触发呢？

冒泡中，内部元素的事件先被触发，然后再外部元素，即： `<p>` 元素的点击事件先触发，然后会触发 `<div>` 元素的点击事件。

捕获中，外部元素的事件会先被触发，然后才会触发内部元素的事件，即： `<div>` 元素的点击事件先触发 ，然后再触发 <p> 元素的点击事件。
`<script>`可以写到`<head><body>`里面，也可以外链文件`<script src="xxx.js"></script>`

<hr>

**作为对象属性的函数被称为 **方法**。**
<hr>
> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbNDIxMTQ1ODkzLDYwOTk4NTU1Ml19
-->