对象：var xxxx={"name“:"xiaobao", "egg”:234 };
数组：
	var yyyy=
	[
		{"name":"ejfhf", "num":238},
		{"name":"fghf", "num":1028},
		{"name":"uiy", "num":323}		
]

字符串：
	var s3=" {\"name\":\"盖伦\"  , \"hp\":616}";

字符串 转换 对象：eval（）
`var gareen = eval("("+s3+")");`
对象 转换 字符串：
`var heroString = JSON.stringify(xxxx);`
> Written with [StackEdit](https://stackedit.io/).
<!--stackedit_data:
eyJoaXN0b3J5IjpbMjMxMjUyOTM4LDU0MDIzMjc4NF19
-->