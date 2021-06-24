对象：var xxxx={"name“:"xiaobao", "egg”:234 };

数组：
	var yyyy=
	[
		{"name":"ejfhf", "num":238},
		{"name":"fghf", "num":1028},
		{"name":"uiy", "num":323}		
]

字符串：
	var s3=' {"name":"盖伦"  , "hp":616} ';

字符串 转换 对象：eval( ) 、 JSON.parse()
`var myObj = JSON.parse(this.responseText);`
`var gareen = eval("("+s3+")");`

对象 转换 字符串： JSON.stringify( )
`var xxxxString = JSON.stringify(xxxx);`

**JSON格式如何与JavaScript数据转换？**
 在向 web 服务器发送数据时，数据必须是字符串，因为可以 直接在JavaScrip中使用JSON语法，所以一般发送数据 和接收数据直接用JSON语法就可。
  也可通过 JSON.stringify() 把 JavaScript 对象转换为字符串， 或者可以使用 JSON.parse() 方法将数据转换为 JavaScript 对象。

**如何使用JSON接收和发送数据？** 
使用 AJAX 或者发送数据，例如： 
var xmlhttp = new XMLHttpRequest(); //创建 XMLHttpReques对象。
 xmlhttp.onreadystatechange = function() { //设置响应函数 
 if (this.readyState == 4 && this.status == 200) { 
 myObj = JSON.parse(this.responseText); 
//responseText获得服务器发送的响应数据。 document.getElementById("demo").innerHTML = myObj.name;
  } }; 
 xmlhttp.open("GET", "json_demo.txt", true);//设置访问页面 xmlhttp.send()；//send一般要包含要发送的数据。

> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbLTk4MTM5NTI1NSwxNjc3MDg4NDEyLC0zNT
U0ODcwMTIsLTE3MzQ3ODM1MTIsLTExNTk1NTg5ODAsNTQwMjMy
Nzg0XX0=
-->