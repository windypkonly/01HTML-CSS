## 01HTML

### 1 什么是HTML

- HTML（Hyper Text Markup Language），超文本标记语言
- HTML用来描述网页的内容和结构，由浏览器负责解析HTML转换成具体的图文界面
- 为什么叫超文本标记语言
  - 由无数个标记（标签、tag)组成HTML代码
  - 由标签和内容组成的称为元素（element）
  - 一般的说法：head元素、\<head>标签，img元素、\<img>标签
- HTML5 是继HTML4.01 和XHTML1.0 之后的超文本标记语言的最新版本

### 2 HTML文件的扩展名

- HTML文件的拓展名是.htm\\.html
  - 历史遗留问题，Win95\Win98系统的文件拓展名不能超过3字符，所以使用.htm

### 3 常用元素

- 区块：div

- 区分：span

- 文本：p、h1~h6、em、dt、dd

- 表格：table、tbody、thead、tr、td、th、tfoot、caption

- 表单：form、input、label、textarea、select

- 链接：a

- 图片：img

- 文档：html、head、title、body、meta

- 列表：ul、ol、li、dlside、footer、nav

- 其他：br、hr、iframe

- 结构：header、section、a、strong、pre、address、q、blockquote、cite、code

### 4 元素的属性

- 每一个元素都可以拥有自己的属性，属性可以增强元素的功能
- 属性名都是小写，而且是无序的，谁先谁后不影响实际效果
- 属性值可以使用双引号、单引号括住，也可以省略引号。建议统一使用双引号

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Document</title>
</head>
<body bgcolor="red" id="main" class="box">

</body>
</html>
```

- 公共属性
  - 有些属性是公共的，每一个元素都可以设置，如：pclass、id、title属性
- 非公共属性
  - 有些属性是元素特有的，如： meta元素的charset属性、img元素的alt属性

### 5 注释

- 对一段代码进行说明

- 语法：<!-- 注释内容 -->

### 6 HTML结构

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Document</title>
</head>
<body>

</body>
</html>
```

- \<!DOCTYPE html>

  - HTML文档声明，告诉浏览器当前页面是HTML5页面，让浏览器用HTML5的标准去解析识别HTML文档
  - 必须放在HTML文档的最前面，不能省略，省略了会出现兼容性问题

- html元素

  - html元素是HTML文档的根元素，一个文档中只能有一个，其他所有元素都是它的后代元素
  - W3C标准建议为html元素增加一个lang属性  
    - 帮助语音合成工具确定要使用的发音
    - 帮助翻译工具确定要使用的翻译规则  
    - lang = "en"  //英文
    - lang = "zh"  //中文

- head元素

  - head元素里面的内容是一些“元数据”（元数据：描述数据的数据）
    - 一般用于描述网页的各种信息，比如字符编码、网页标题、网页图标
  - title元素
    - 网页的标题
  - meta元素
    - 用于设置网页的字符编码，让浏览器更精准地显示每一个文字，不设置或者设置错误会导致乱码  
    - 一般都使用UTF-8编码，涵盖了世界上几乎所有的文字
  - style

  - link

  - base

  - script

  - noscritpt

- body元素

  - body元素里面的内容将是你在浏览器窗口中看到的东西，也就是网页的具体内容和结构

