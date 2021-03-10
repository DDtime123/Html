# 这是关于html的学习总结

------

html是一种标记语言，通过浏览器内核的解析执行，用于创建网页。

## Html 网页结构
```html
<!DOCTYPE html>
<html>
<head>
<title> html基本页面结构 </title>
</head>
<body></body>
</html>
```
```<!DOCTYPE html/```是文档的声明头，他告诉浏览器这里是一份Html文档。```<html>```是根元素，一切文本的开头。```<head>```是头元素，头元素里摆放一些不在主页面中显示的内容，如```<title>```页面的标题，css文件的引用等。```<body>```是主题元素，页面内一切内容都放在```<body>```里。

### Html 注释
Html采用```<!-- -->```符号进行注释，```<!-- -->```可以在任何文本之间，符号内的内容将不会在页面上显示。

## Html 标签
Html 通过标签声明文章的结构，文本的格式，它就是构成Html 网页的钢筋水泥。
### 标签
标签分为单标签和双标签。
#### 双标签
```<标签名></标签名>```
* ```<div>```：区块标签，用于分隔页面。
* ```<a>```：超链接标签，用于跳转到下一个页面，格式为```<a href="URL">连接的描述</a>```。
* ```<h1>```：标题标签，有 ```<h1>``` 至 ```<h6>``` 6种标签，其中数字越小，标题文字越大。
* ```<p>```：段落标签。
* ```<ul>```：列表标签，格式为
```
<ul>
    <li>元素1</li>
    <li>元素2</li>
</ul>
```
#### 单标签
```</标签名>```
* ```<br/>```：强制换行
* ```<hr/>```：下划线
* ```<meta/>```：声明网页所使用字符集标签，例如 ```<meta charset="UTF-8"/>```
* ```<img/>```：插入图片标签
* ```<input/>```：输入标签

## Html 表单
```<form>```：表单标签
Html 的表单是网页用于和服务器交换数据的模块，其中 ```action``` 是表单数据传输的方式，它的取值有 ```post``` 和 ```get``` 两种，其中 ```post``` 方式更为安全，一般用于传递账户密码等信息， ```get``` 中信息会在 URL 中显示，容易被看见。
```html
<form action="" method="" name="">
    <input type="typename" name="dataname" value="">
</form>
```

### Html 输入标签
```html
<!-- input标签 -->
<!-- 可配合 type 属性，搭配不同元素以实现不同的输入方式 -->
<!-- 如搭配 "checkbox" 元素，它就是个多选框-->
<!-- 搭配 "audio" 元素，它是个单选框（前提是设置 name 属性，并将 name 设置为相同值）-->
<!-- 搭配 "button" 元素可实现与 <button> 相同的按钮输入方式  -->
<input type="" name="" value=""/>
<!-- button标签 -->
<button></button>
<!-- select标签 -->
<select>
    <!-- 下拉列表 -->
    <option>元素1</option>
    <option>元素2</option>
</select>
<!-- select标签 -->
```

## Html 表格
```<table>```：表格标签
用于在网页上生成表格
```html
<table>
    <caption>表格名</caption>
    <tr>
        <th>字段1</th>
        <th>字段2</th>
        <th>字段2</th>
    </tr>
    <tr>
        <td>元素1</td>
        <td>元素2</td>
        <td>元素3</td>
    </tr>
    <tr>
        <td>元素1</td>
        <td>元素2</td>
        <td>元素3</td>
    </tr>
</table>
```
其表现为：
<table>
    <caption>表格名</caption>
    <tr>
        <th>字段1</th>
        <th>字段2</th>
        <th>字段2</th>
    </tr>
    <tr>
        <td>元素1</td>
        <td>元素2</td>
        <td>元素3</td>
    </tr>
    <tr>
        <td>元素1</td>
        <td>元素2</td>
        <td>元素3</td>
    </tr>
</table>

