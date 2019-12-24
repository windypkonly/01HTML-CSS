## 02 HTML基础元素

### 1 基础元素

- \<h>元素
  - 表示网页的标题
  - h1~h6共规定了6个等级的标题

- \<p>元素
  - 表示文章中的一个段落 （paragraph）

  - h元素和SEO

    - h元素有助于网站的SEO（Search Engine Optimization）优化，可以促进关键词排名

    - 建议在网页中最多只有1个h1元素

    - 乱用h元素不仅不会给网站带来好的权重，同时也有可能被搜索引擎认为作弊，最后导致K站

-  \<strong>元素
  - 用于强调某些文本，粗体的显示效果

- \<div>元素
  - 块级元素
  - 一般作为其他元素的父容器，把其他元素包住，代表一个整体
  - 用于把网页分割为多个独立的部分

- \<span>元素
  - 行内元素
  - 默认情况下，跟普通文本几乎没差别
  - 用于区分特殊文本和普通文本，比如用来显示一些关键字
- \<code>元素
  - 用于显示程序代码
- \<br>元素
  - 单标签，表示强制换行，一般不使用，换行内容使用div包住
- \<hr>元素
  - 分割线，一般不使用，分割线用css样式进行控制

### 2 字符实体

- HTML实体就是将有特殊意义的字符通过实体代码显示出来。

|      | 描述            | 实体名称 | 实体编号 |
| ---- | --------------- | -------- | -------- |
|      | 空格            | &nbsp;   | &#160;   |
| <    | 小于号          | &lt;     | &#60;    |
| >    | 大于号          | &gt;     | &#62;    |
| &    | 和号            | &amp;    | &#38;    |
| "    | 双引号          | &quot;   | &#34;    |
| '    | 单引号          | &apos;   | &#39;    |
| ￠   | 分(cent)        | &cent;   | &#162;   |
| £    | 镑(pound)       | &pound;  | &#163;   |
| ¥    | 元(yen)         | &yen;    | &#165;   |
| €    | 欧元(euro)      | &euro;   | &#8364;  |
| §    | 小节            | &sect;   | &#167;   |
| ©    | 版权(copyright) | &copy;   | &#169;   |
| ®    | 注册商标        | &reg;    | &#174;   |
| ™    | 商标            | &trade;  | &#8482;  |
| ×    | 乘号            | &times;  | &#215;   |
| ÷    | 除号            | &divide; | &#247;   |

### 3 img元素

- img元素（image的缩写），单标签，专门用来显示图片

- src属性（source的缩写）用来设置图片的路径（URL）

  - 相对路径：完整的描述文件位置的路径
  - 绝对路径：由当前文件所在的文件夹引起的跟其它文件的路径关系  
    - ./ 代表当前文件夹，可以省略
    - ../ 代表上级文件夹
  - 对于网页来说，不管什么操作系统（Windows、Mac、Linux），路径分隔符都是 /，而不是 \

- 注意

  - img元素如果只设置了width（或height），浏览器会自动根据图片宽高比计算出height（或width）
  - 在HTML5规范中，alt是img元素的必要属性

  - width、height的默认单位是px，像素

### 4 a元素

- a元素用于定义超链接，用于打开新的URL

- 常用属性

  - href（Hypertext Reference）：指定要打开的URL

  - ptarget：打开URL的位置

    - _self：默认值，在当前窗口打开URL

    - _blank：在一个新的窗口中打开URL

    - _parent：在父窗口中打开URL

    - _top：在顶层窗口中打开URL

    - 某个frame的name值：在某个frame中打开URL

- iframe元素

  - src：指定要打开的URL
  - frameborder属性：用于规定是否显示边框（1表示显示，0表示不显示） 

- base元素

  - base元素写在head元素中
  - 利用base元素设置当前页面所有a元素的默认行为  

- 锚点链接

  - 锚点链接可以实现：跳转到网页中的具体位置

```html
    <br><br><br><br><br><br><br><br><br><br>
    <p id="one">第1节</p>
    <br><br><br><br><br><br><br><br><br><br>
    <br><br><br><br><br><br><br><br><br><br>
    <br><br><br><br><br><br><br><br><br><br>
    <br><br><br><br><br><br><br><br><br><br>
    <br><br><br><br><br><br><br><br><br><br>
    <p id="two">第2节</p>
    <br><br><br><br><br><br><br><br><br><br>
    <br><br><br><br><br><br><br><br><br><br>
    <br><br><br><br><br><br><br><br><br><br>
    <br><br><br><br><br><br><br><br><br><br>
    <br><br><br><br><br><br><br><br><br><br>
    <a href="#one">回到【第1节】</a>
    <a href="#two">回到【第2节】</a>
    <a href="#">回到【最顶部】</a>
```

- 伪链接

```html
    <a href="">百度一下</a>
    <a href="" onclick="alert('Hello World');">Hello World</a>
    <a href="javascript: alert('Hello HTML')">Hello HTML</a>
```

- 图片链接

```html
    <a href="http://www.baidu.com">
        <img src="./img/yuzhou_01.jpg" alt="">
    </a>
```

