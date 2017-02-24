form 表单向后台提交数据
=====================

```html
	
	<!DOCTYPE html>
	<html lang="en">
	<head>
	  <meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1, user-scalable=no">
	  <meta charset="UTF-8">
	  <title>formData</title>
	</head>
	<body>
		<form action="" enctype="multipart/form-data" method="POST">
			<input type="file" multiple name="image">
			<input type="text" name="data" value="Jack">
		</form>
	</body>
	</html>

```

> form表单提交数会用到的主要属性：
> 
> * action-要提交数据的服务器地址
> * method-如何发送表单数据（get/post）
> * enctype-规定在发送服务器之前应该如何对表单数据进行编码（默认，表单数据编码为‘application/x-www-form-urlencoded’，即在发送服务器之前，所有字符都会进行编码（空格转换为 “+” 加号，特殊符号转换为ASCII HEX值））。
> 
> <table>
>	<tr>
>		<td>enctype值</td>
>		<td>描述</td>
>	</tr>
>	<tr>
>		<td>application/x-www-form-urlencoded</td>
>		<td>在发送前编码所有字符（默认）</td>
>	</tr>
>	<tr>
>		<td>multipart/form-data</td>
>		<td>不对字符编码。在使用包含文件上传控件的表单时，必须使用>该值。</td>
>	</tr>
>	<tr>
>		<td>text/plain</td>
>		<td>空格转换为 "+" 加号，但不对特殊字符编码。</td>
>	</tr>
> <table>

##### tips
> 上传文件类内容数据，应开启form表单的 enctype="multipart/form-data",并选择method="POST"进行数据的提交
>
[更多关于form的属性介绍-W3school-form标签](http://www.w3school.com.cn/tags/tag_form.asp)

