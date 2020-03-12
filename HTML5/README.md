# 第一章 介绍
## 开始学习 HTML
HTML 指的是超文本标记语言（英语：HyperText Markup Language），是用来描述网页的一种语言。
*   HTML 不是一种编程语言，而是一种标记语言，它有一套标记标签 。
*   HTML 使用标记标签来描述网页。
*   HTML 文档包含了 HTML 标签及文本内容，HTML文档也叫做 Web 页面。
您可以使用 HTML 来建立自己的 Web 站点，HTML 运行在浏览器上，由浏览器来解析。  
在本课程中，您将学习如何使用 HTML 来创建站点。
## HTML 网页结构
下面是一个可视化的 HTML 页面结构实例：
```angular2  
<html>
   <head>
   <title>页面标题</title>
   </head>
   <body>
     <h1>这是一个标题。</h1>
     <p>这是一个段落。</p>
   </body>
</html>
   
```


**我们来解析一下**  
```angular2
<html> 与 </html> 之间的文本描述网页。
<head> 与 </head> 之间的文本描述文档的元数据。
<title> 与 </title> 之间的文本描述文档的标题。
<body> 与 </body> 之间的文本是可见的页面内容。
<h1> 与 </h1> 之间的文本被显示为一个大标题。
<p> 与 </p> 之间的文本被显示为一个段落。
```
只有body区域才会在浏览器中显示，显示效果如下图：  
![图片](img/img1.jpg)

## html 标签
html 元素定义了整个 HTML 文档。  
这个元素拥有一个开始标签html ，以及一个结束标签/html。
```angular2
<html>
 …
</html>
```

## head 标签
head 元素包含了所有的头部标签元素。  
head  元素必须包含文档的标题（title），可以包含脚本、样式、meta 信息以及其他更多的信息。
```angular2
    <html>
      <head>…</head>
    </html>
```
## body 标签
body 元素定义文档的主体。  
body 元素包含文档的所有内容（比如文本、超链接、图像、表格和列表等等）。  
下面是 HTML 的基本结构：
```angular2
<html>
  <head>…</head>
  <body>
  …
  </body>
</html>

```
## HTML 编辑器
HTML 文件是文本文件，因此你可以使用任何文本编辑器来创建 HTML 文件。  
有一些很不错的 HTML 编辑器可用，你可以选择适合你自己的那个。W3Cschool 为大家推荐几款常用的编辑器：  
* **Notepad++：** [Notepad++](https://notepad-plus-plus.org/)
* **Sublime Text：** [Sublime Text](http://www.sublimetext.com/)
* **VS Code：** [VS Code](https://code.visualstudio.com/)  
你可以从以上软件的官网中下载对应的软件，按步骤安装即可。  
## 创建 HTML 文件
接下来，我们将演示如何使用 Sumlime Text 编辑器来创建 HTML 文件。
***
**步骤 1：新建 HTML 文件**  
在 Sublime Text 安装完成后，选择" 文件(F)->新建(N) "，在新建的文件中输入以下代码：
```angular2
<!DOCTYPE html>
<html>
<head>
<meta charset="utf-8">
<title>w3cschool - 随时随地学编程</title>
</head>
<body>
  <h1>我的第一个标题。</h1>
  <p>我的第一个段落。</p>
</body>
</html>
```
如下图所示：
![图片](img/img2.png)  
> 提示：对于中文网页需要使用 `````<meta charset="utf-8">````` 声明编码，否则会出现乱码。有些浏览器（如 360 浏览器）会设置 GBK 为默认编码，则你需要设置为 <meta charset="gbk">。
## 保存 HTML 文件
### 步骤 2：另存为 HTML 文件
然后选择" 文件(F)->另存为(A) "，文件名为 first.html。  
如下图所示：
![图片](img/img3.jpg)  
当您保存 HTML 文件时，既可以使用 .htm 也可以使用 .html 后缀名。两种后缀名没有区别，完全根据您的喜好，推荐使用 .html。
## 运行 HTML 文件
### 步骤 3：在浏览器中运行这个 HTML 文件
启动您的浏览器，然后选择" 文件 "菜单的" 打开文件 "命令，或者直接在文件夹中双击您的 HTML 文件。  
运行显示结果如下图：  
![图片](img/img4.png)
## 代码初体验，制作第一个网页
### 任务：请你试一试，制作你的第一个网页。  
给p元素之间添加文本“你好HTML”。显示如下图所示：
![图片](img/img5.jpg)
## HTML 元素
HTML 文档由 HTML 元素定义。  
HTML 元素```以开始标签起始，以结束标签终止，元素的内容是开始标签与结束标签之间的内容。```   
HTML 文档由嵌套的 HTML 元素构成。  
```实例:``` 这个 HTML 文档包含了三个 HTML 元素。
```angular2
<html>
  <body>
    <p>这是第一个段落。</p>
  </body>
</html>
```
## HTML 空元素
没有内容的 HTML 元素被称为空元素。空元素是在开始标签中关闭的。  
例如，`````<br>````` 就是没有关闭标签的空元素，`````<br>````` 标签定义折行（换行）。  
在开始标签中添加斜杠，比如 ```<br />```，是关闭空元素的正确方法。  
```angular2
<html>
  <body>
    <p>这是一个段落。</p>
    <p>这是一个<br />换行。</p>
  </body>
</html>
```  
> **提示：** 即使 ```<br>``` 目前在所有浏览器中都是有效的，但为了获得更长远的保障，w3cschool 建议使用 ```<br />```。
## HTML 属性
*属性* 是 HTML 元素提供的附加信息。
+ HTML 元素可以设置属性
+ 属性可以在元素中添加附加信息
+ 属性一般描述于开始标签
+ 属性总是以名称/值对的形式出现，比如：name="value"。
### 属性实例：
这是一个链接使用了 href 属性。  
```angular2
<a href="http://www.w3cschool.cn">这是一个链接</a>
```
## HTML 属性值
属性值应该始终被包括在```引号内```。  
``双引号``是最常用的，不过使用单引号也没有问题。  
在某些个别的情况下，比如属性值本身就含有双引号，那么您必须使用单引号，例如：
```angular2
name='Bill "HelloWorld" Gates'
```
> ```提示：```属性和属性值对大小写不敏感。不过，推荐标准中推荐小写的属性/属性值。  
## HTML 常用的属性
下面列出了 HTML 常用的属性，适用于大多数 HTML 元素。   
*** 
> |属性|描述|
|:--------- |:------- |
|class			|为 html 元素定义一个或多个类名（类名从样式文件引入）
|id				|定义元素的唯一 id
|style			|规定元素的内联样式
|title	    	|规定元素的额外信息（可在工具提示中显示）
## HTML class 与 id 属性
### class 属性 
class 属性为 HTML 元素定义一个或多个类名。  
class 属性通常用于指向样式表中的类。 
#### 例子：
```
<p class="intro">这是一个段落。</p>
```
### id 属性
id 属性定义 HTML 元素的唯一的 id。  
id 在 HTML 文档中必须是唯一的。 
#### 例子：
```angular2
<h1 id="header">w3cschool</h1>
```
# 第二章 HTML 基础
## HTML 标题
HTML 标题（Heading）是通过 ```<h1> - <h6>``` 标签进行定义的。  
根据重要性排列，```<h1>``` 定义最大的标题，```<h6>``` 定义最小的标题。  
下面的实例定义了所有标题。
```angular2
<h1>这是标题 1</h1>
<h2>这是标题 2</h2>
<h3>这是标题 3</h3>
<h4>这是标题 4</h4>
<h5>这是标题 5</h5>
<h6>这是标题 6</h6>
```
在浏览器中显示如下  
![图片](img/img6.jpg)
> ### 提示：
> 用户可以通过标题来快速浏览您的网页，所以用标题来呈现文档结构是很重要的。  
> 应该将 h1 用作主标题（最重要的），其后是 h2（次重要的），再其次是 h3，以此类推。
## HTML 水平线
```<hr />``` 是一个空元素，这里的“hr”是“水平线（horizontal rule）”的意思。  
```<hr />``` 标签在 HTML 页面的作用是创建水平线。  
```<hr />``` 元素可用于分隔 HTML 页面中的内容。
```angular2
<hr />
<p>这是一个段落。</p>

<hr />
<p>这是另一个段落。</p>
```
## HTML 注释
我们可以将注释插入 HTML 代码中，这样可以提高其可读性，使代码更易被人理解。  
但浏览器会忽略注释，也不会显示它们。
### HTML 注释写法如下：
```angular2
<!-- 这是一个注释 --> 
```
在添加注释时，开始括号之后（左边的括号）需要紧跟一个叹号，但结束括号之前（右边的括号）不需要。
> 提示：合理地使用注释可以对未来的代码编辑工作产生帮助。
## 使用 ```<h2>``` 标签显示标题
> 任务：请你试一试，亲自感受下 ```<h2>``` 标签的使用。  

在h1元素下面创建一个h2元素，h2元素里面的文本为“你好HTML”。显示如下图所示：
![图片](img/img7.jpg)
## HTML 段落
创建段落，是通过 ```<p>``` 标签定义的。
### 实例：
```angular2
<p>这是一个段落。</p>
<p>这是另一个段落。</p>
```
在浏览器中显示如下：  
![图片](img/img8.jpg)
> 提示：浏览器会自动地在段落的前后添加空行。  
## HTML 折行
如果你希望在不产生一个新段落的情况下进行折行（换行），请使用 ```<br>``` 标签。  
```<br>``` 标签是一个空标签，意味着它没有结束标签。
### 实例：
```angular2
<p>这是一个段落。</p>
<p>这是另一个段落。</p>
<p>这个段落<br>演示了折行（换行）的效果。</p>
```
在浏览器中显示如下：  
![图片](img/img9.jpg)
> #### 提示：
> 请使用 ```<br>``` 标签来输入空行，而不是分割段落。
> 在写地址信息或者写诗词时 <br> 标签非常有用。
## HTML 格式化标签
HTML 使用 ```<b>``` 标签与 ```<i>``` 标签对输出的文本进行格式化，用来定义 **粗体** 和 *斜体*。  
这些 HTML 标签被称为格式化标签。
### 下面是常用的 HTML 文本格式化标签。
![图片](img/img10.jpg)
## HTML 文本格式化标签
下面是一个 HTML 文本格式化的实例。  
每个段落都运用了不同的格式化标签，来演示每个标签的作用。
```angular2
 <p><b>定义粗体文本</b></p>
 <p><em>定义着重文字</em></p>
 <p><i>定义斜体字</i></p>
 <p><small>定义小号字</small></p>
 <p><strong>定义重要的文本</strong></p>
 <p>定义<sub>下标字</sub></p>
 <p>定义<sup>上标字</sup></p>
 <p><ins>定义插入字</ins></p>
 <p><del>定义删除字</del></p>
```
在浏览器中显示如下：  
![图片](img/img11.jpg)
## ```<a>``` 标签
HTML 使用 ```<a>``` 标签来设置超文本链接。  
超链接可以是一个字，一个词，或者一组词，也可以是一幅图像，你可以点击这些内容来跳转到新的文档或者当前文档中的某个部分。  
在 ```<a>``` 标签中，使用 href 属性来描述链接的目标地址。  
链接的 HTML 代码很简单。它类似这样
```angular2
<a href="url">链接文本</a>
```
## 创建超链接
在下面的例子中，定义了 w3cschool 网站的超链接，点击这个超链接会把你带到 w3cschool 的首页。
```angular2
<a href="https://www.w3cschool.cn">访问w3cschool</a>
```
在浏览器中显示如下：
![图片](img/img12.jpg)
默认情况下，链接将以以下形式出现在浏览器中： 
+ 一个未访问过的链接显示为蓝色字体并带有下划线。
+ 访问过的链接显示为紫色并带有下划线。
+ 点击链接时，链接显示为红色并带有下划线。
> 提示：如果为这些超链接设置了 CSS 样式，展示样式会根据 CSS 的设定而显示。
##  HTML <a> target 属性
在 <a> 标签中使用 target 属性，你可以规定在何处打开链接文档。  
target 属性值有：
+ _blank：在新窗口中打开被链接文档。
+ _self：默认。在相同的框架中打开被链接文档。
+ _parent：在父框架集中打开被链接文档。
+ _top：在整个窗口中打开被链接文档。
+ framename：在指定的框架中打开被链接文档。  
实例：下面的链接会在新窗口打开文档。
```angular2
<a href="https://www.w3cschool.cn" target="_blank">访问w3cschool</a>
```
## 使用 <a> 标签链接到另一个页面
### 任务：请你试一试，亲自感受下 <a> 标签的使用。
在p元素下方创建一个a元素，并为a元素添加href属性，使其指向此URL：  
https://www.w3cschool.cn，再添加target属性的值为 _blank ，使链接在新窗口中打开，a元素里面的文本为“访问w3cschool。显示如下图所示：
![图片](img/img13.jpg)
## HTML ```<head>``` 元素
```<head>``` 元素包含了所有的头部标签元素。  
在 ```<head>```元素中你可以插入脚本（scripts）, 样式文件（CSS），及各种meta信息。  
可以添加在头部区域的元素标签为：```<title>, <style>, <meta>, <link>, <script>, <noscript>,<base>```。

****
### 下面是 ```<head>``` 元素包含的头部标签元素列表：
![图片](img/1.jpg)
> 提示：不要担心本节中您还没有学过的标签，您将在接下来的小节中学到它们。
## ```<title>``` 元素
```<title>``` 标签定义了 HTML 文档的标题，在所有 HTML 文档中是必需的。  
```<title>``` 元素：
+ 定义浏览器工具栏中的标题
+ 提供页面被添加到收藏夹时的标题
+ 显示在搜索引擎结果中的页面标题
```
<html>
   <head>
       <title>…</title>
   </head>
</html>
```
## HTML CSS介绍
CSS （层叠样式表又称为级联样式表，英文 Cascading Style Sheets 的缩写）是用于渲染 HTML 元素标签的样式。  
CSS 是 HTML 的搭档。在编码过程中，它们发挥不同的作用：
+ HTML 负责网页的具体内容（结构）
+ CSS 则修饰网页的表现形式（布局）  
CSS 可以通过以下方式添加到HTML中：
+ 内联样式：在HTML元素中使用“style”属性。
+ 内部样式表：在HTML文档头部 ```<head>``` 区域使用 ```<style>``` 元素来包含 CSS。
+ 外部引用：使用外部CSS文件。
> 最好的方式是通过外部引用CSS文件。  
> 提示：您可以通过 CSS 微课 学习更多的 CSS 知识。
## 内联样式
当特殊的样式需要应用到个别元素时，就可以使用内联样式。   
使用内联样式的方法是在相关的标签中使用样式属性。样式属性可以包含任何 CSS 属性。  
### 内联样式实例：
我们使用font-family（字体），color（颜色），和font-size（字体大小）属性来定义字体的样式。
```angular2
<h1 style="font-family:arial;">w3cschool</h1>
<p style="font-family:arial;color:red;font-size:20px;">随时随地学编程</p>
```
在浏览器中显示如下：  
![图片](img/2.jpg)
## HTML 内联样式实例
使用 text-align（文字对齐）属性指定文本的水平与垂直对齐方式：
```angular2
<!DOCTYPE html>
<html>
<head> 
<meta charset="utf-8"> 
<title>内联样式实例 - w3cschool</title> 
</head>
<body>

<h1 style="text-align:center;">居中对齐的标题</h1>
<p>这是一个段落。</p>
```
## 内部样式表
当单个文件需要特别样式时，就可以使用内部样式表。你可以在```<head>``` 部分通过 ```<style>```标签定义内部样式表。
### 内部样式表实例：
我们在 HTML 文档中使用 ```<style>``` 元素。 
```angular2
<head>
<style type="text/css">
 h1 {color:red;}
 p {color:blue;}
</style>
</head>
```
在浏览器中显示如下：  
![图片](img/3.png)
## 外部样式表
当样式需要被应用到很多页面的时候，外部样式表将是理想的选择。使用外部样式表，你就可以通过更改一个文件来改变整个站点的外观。
### 外部样式表实例：
```angular2
<head>
<link rel="stylesheet" type="text/css" href="/statics/demosource/styles.css">
</head>
```
在浏览器中显示如下：
![图片](img/4.png)
## ```<img>``` 标签
在 HTML 中，图像由 ```<img>``` 标签定义。  
```<img>``` 是空标签，它只包含属性，并且没有闭合标签。  
要在页面上显示图像，你需要使用源属性（src）。源属性的值是图像的 URL 地址。
### 定义图像的语法是：
```angular2
<img src="url">
```
## 图像位置
URL 指存储图像的位置，你需要为位于引号之间的 src 属性放置图像位置。  
例如， 如果名为 "index-logo.png" 的图像位于 www.w3cschool.cn 的 images 目录中，那么其 URL 为  
https://www.w3cschool.cn/images/index-logo.png。  
### 实例：
```angular2
<img src="index-logo.png">
```
在浏览器中显示如下：
![图片](img/5.png)
## 图像 alt 属性
**alt** 属性用来为图像定义一串预备的可替代的文本。  
替代文本属性的值是用户定义的。
### 例如：
```angular2
<img src="index-logo.png" alt="随时随地学编程">
```
在浏览器无法载入图像时，替代文本属性告诉读者他们失去的信息。此时，浏览器将显示这个替代性的文本而不是图像。 
> 提示：为页面上的图像都加上替换文本属性是个好习惯，这样有助于更好的显示信息，并且对于那些使用纯文本浏览器的人来说是非常有用的。
## 设置图像的宽度与高度
width（宽度）与 height（高度）属性用于设置图像的宽度与高度。  
width 与 height 属性值可以以 px（像素）或 %（百分比）形式指定，默认单位为 px（像素）。  
### 实例：
```angular2
<img src="index-logo.png" alt="随时随地学编程" width="228" height="60">
```
在浏览器中显示如下：
![图片](img/6.png)
## HTML 无序列表
HTML 支持有序列表、无序列表和自定义列表。  
无序列表是一个项目的列表，此列项目使用粗体圆点（典型的小黑圆圈）进行标记。  
```<ul>``` 标签定义无序列表。将`` <ul>`` 标签与```<li>``` 标签一起使用，创建无序列表。  
实例：下面是一个无序列表。
```angular2
<ul>
  <li>苹果</li>
  <li>香蕉</li>
  <li>菠萝</li>
</ul> 
```
在浏览器中显示如下：  
![图片](img/7.png)
## HTML 有序列表
有序列表也是一列项目，列表项目使用数字进行标记  
```<ol>``` 标签定义了一个有序列表，列表排序以数字来显示。使用 ```<li>``` 标签来定义列表选项。  
实例：下面是个有序列表。
```angular2
<ol>
  <li>苹果</li>
  <li>香蕉</li>
  <li>菠萝</li>
</ol> 
```
在浏览器中显示如下：  
![图片](img/9.png)  
## HTML 自定义列表
自定义列表不仅仅是一列项目，而是项目及其注释的组合。  
自定义列表以 ```<dl>``` 标签开始。每个自定义列表项以 ```<dt>``` 开始。每个自定义列表项的描述以 ```<dd>``` 开始。  
实例：下面是一个自定义列表。  
```angular2
<dl>
  <dt>苹果</dt>
    <dd>又大又红</dd>
  <dt>香蕉</dt>
    <dd>又香又甜</dd>
</dl>
```
在浏览器中显示如下：  
![图片](img/10.png)
## HTML 块级元素
大多数 HTML 元素被定义为**块级元素**或**内联元素**。
---
HTML 区块元素  
块级元素在浏览器显示时，通常会以新行来开始（和结束）。  
例如： ```<div>, <h1>, <p>, <ul>, <table>``` 元素。
### 实例：
```angular2
<h1>w3cschool</h1>
<p>随时随地学编程</p>
```
在浏览器中显示如下：  
![图片](img/11.png)
## HTML 内联元素
内联元素在显示时通常不会以新行开始。  
例如：`````<span>, <a>, <img>, <b>, <td>````` 元素。
### 实例：
```angular2
<span>红色</span>
<span>蓝色</span>
<span>绿色</span>
```
在浏览器中显示如下：   
![图片](img/12.png)
## HTML ```<div>``` 元素  
```<div>``` 元素是块级元素，它可用于组合其他 HTML 元素的容器。
```<div>``` 元素没有特定的含义。除此之外，由于它属于块级元素，浏览器会在其前后显示折行（换行）。  
如果与 CSS 一同使用，<div> 元素可用于对大的内容块设置样式属性。  
实例：文档中的 ```<div>``` 元素区域将显示为红色。
```angular2
<div style="color:#FF0000">
  <h1>这是一个在 div 元素中的标题。</h1>
  <p>这是一个在 div 元素中的文本。</p>
</div>
```
在浏览器中显示如下：  
![图片](img/13.png)  
> 提示：```<div>``` 元素的另一个常见的用途是文档布局。它取代了使用表格定义布局的老式方法。
## HTML ```<span>``` 元素
```<span>``` 元素是内联元素，可用作文本的容器。  
```<span>``` 元素也没有特定的含义。  
当与 CSS 一同使用时，<span> 元素可用于为部分文本设置样式属性。  
实例：使用 <span> 元素对文本中的一部分进行设置样式。
```angular2
<p>我的哥哥有 <span style="color:0000FF;font-weight:bold">蓝色</span> 的球鞋，我的姐姐有 <span style="color:FF0000;font-weight:bold">红色</span> 的球鞋。</p>
```
在浏览器中显示如下：
![图片](img/14.png)
## ```<iframe>``` 标签
通过使用框架，你可以在同一个浏览器窗口中显示不止一个页面。  
```<iframe>``` 标签规定一个内联框架。  
一个内联框架被用来在当前 HTML 文档中嵌入另一个文档。  
实例：标记一个内联框架。
```angular2
<iframe src="https://www.w3cschool.cn"></iframe>
```
在浏览器中显示如下：
![图片](img/15.png)  
> 提示：你可以把需要的文本放置在 ```<iframe> 和 </iframe>``` 之间，这样就可以应对不支持 ```<iframe> 的浏览器（一些旧的浏览器不支持iframe）```。
## 定义 ```<iframe>``` 标签的高度与宽度
height 和 width 属性用来定义 ```<iframe>``` 标签的高度与宽度。  
属性默认以 px（像素）为单位，但是你可以指定其按比例显示 (如："90%")。
### 实例：   
```angular2
<iframe src="/statics/demosourse/demo_iframe.htm" width="300" height="300"></iframe>
```
在浏览器中显示如下：  
![图片](img/16.png)
## 定义 ```<iframe>``` 标签是否显示边框
frameborder 属性用于定义 ```<iframe>``` 是否显示边框。  
frameborder 属性默认值为“1”，表示开启边框。设置 frameborder 属性值为 "0" ，则表示移除 ```<iframe>``` 的边框。
### 实例：
```angular2
<iframe src="/statics/demosourse/demo_iframe.htm" width="300" height="300" frameborder="0">
```
在浏览器中显示如下：
![图片](img/17.png)  
> 提示：HTML5 不支持 ```<iframe>``` frameborder 属性，请使用 CSS 设置样式代替。
## HTML 颜色
HTML 颜色由一个十六进制符号来定义，这个符号由红色、绿色和蓝色的值组成（RGB）。  
每种颜色的最小值是 0（十六进制：#00），最大值是 255（十六进制：#FF）。  
RGB 模型如下图所示：  
![三原色](img/rgb.jpg)
## HTML 颜色值
HTML 三种颜色 红，绿，蓝的组合从 0 到 255，一共有1600万种不同颜色(256 x 256 x 256)。  
下面的表格给出了由三种颜色混合而成的具体效果，不同的值都显示了不同的颜色。  
![颜色值](img/ysz.png)
## HTML 脚本标签
向 HTML 添加脚本，使HTML 页面具有更强的动态性和交互性。  
下面是 HTML 的脚本标签：  
![脚本标签](img/jb.png)
> 提示：学习更多关于 Javascript 知识，请查看 JavaScript 微课。
## HTML ```<script>``` 标签
```<script>``` 标签用于定义客户端脚本，比如 JavaScript。  
```<script>``` 元素既可包含脚本语句，也可通过 src 属性指向外部脚本文件  
JavaScript 最常用于图片操作、表单验证以及内容动态更新。  
实例：下面的脚本会向浏览器输出"Hello W3Cschool!"：
```angular2
<script>
document.write("Hello W3Cschool!");
</script>
```
在浏览器中显示如下：  
![js展示](img/jiaob.png)
## HTML ```<noscript>``` 标签
```<noscript>``` 标签提供无法使用脚本时的替代内容，比方在浏览器禁用脚本时，或浏览器不支持客户端脚本时。  
```<noscript>``` 元素可包含普通 HTML 页面的 body 元素中能够找到的所有元素。  
只有在浏览器不支持脚本或者禁用脚本时，才会显示 <noscript> 元素中的内容。  
### 实例：
```angular2
<script>
document.write("Hello W3Cschool!")
</script>
<noscript>抱歉，您的浏览器不支持 JavaScript!</noscript>
```
在浏览器中显示如下：  
![图片](img/18.png)
## HTML 实体
在 HTML 中，某些字符是预留的。  
在 HTML 中不能使用小于号（<）和大于号（>），这是因为浏览器会误认为它们是标签。  
如果希望正确地显示预留字符，我们必须在 HTML 源代码中使用字符实体。一些在键盘上找不到的字符也可以使用字符实体来替换。  
### 字符实体类似这样：
```angular2
&entity_name;
或
&#entity_number;
```
比如说显示小于号，我们必须这样写：&lt; 或 &#60。 
## HTML 字符实体
HTML 中的常用字符实体是不间断空格（&nbsp;）。  
如果您在文本中按 4 个空格，在显示该页面之前，浏览器会删除它们中的 3 个。如需在页面中增加空格的数量，您需要使用 &nbsp; 字符实体。  
下面是常见的 HTML 实体列表：  
![字符集](img/zfj.png)
> 提示：虽然 HTML 不区分大小写，但实体名称对大小写敏感。
# 第三章 表格
## HTML 表格介绍
HTML 表格由 ```<table>``` 标签来定义。  
一个 HTML 表格包括 ```<table>``` 元素，一个或多个 ```<tr>```、```<th>``` 以及 ```<td>``` 元素。  
```<tr>``` 元素定义表格行，```<th>``` 元素定义表头，```<td>``` 元素定义表格单元。  
实例：下面是一个包含两行三列的表格。
```angular2
<table border="1">
    <tr>
        <td>row 1, cell 1</td>
        <td>row 1, cell 2</td>
	<td>row 1, cell 3</td>
    </tr>
    <tr>
        <td>row 2, cell 1</td>
        <td>row 2, cell 2</td>
	<td>row 2, cell 3</td>
    </tr>
</table>
```
在浏览器中显示如下：  
![表格](img/biao.png)
## HTML 表格标签
HTML 表格常用的标签有 ```<table>、<tr>、<th>、<td>``` 标签。  
更复杂的 HTML 表格也可能包括 ```<caption>、<col>、<colgroup>、<thead>、<tfoot> 以及 <tbody>``` 标签，我们只需要大概了解一下定义。  
下面是 HTML 表格标签描述列表：
![表格标签](img/biao1.png)
## HTML 表格边框属性
border 属性规定表格单元周围是否显示边框。  
如果不定义边框属性，表格将不显示边框。  
border 属性值为 "1" 显示表格的边框是 1 像素宽。  
实例1：下面是一个带有边框的表格。
```angular2
<table border="1">
    <tr>
        <td>苹果</td>
        <td>香蕉</td>
	<td>樱桃</td>
    </tr>
    <tr>
        <td>葡萄</td>
        <td>柠檬</td>
	<td>草莓</td>
    </tr>
</table>
```
在浏览器中显示如下：  
![表](img/biao2.png)  
实例2：下面是一个没有边框的表格。
```angular2
<table>
    <tr>
        <td>苹果</td>
        <td>香蕉</td>
	<td>樱桃</td>
    </tr>
    <tr>
        <td>葡萄</td>
        <td>柠檬</td>
	<td>草莓</td>
    </tr>
</table>
```
在浏览器中显示如下：  
![表](img/biao3.png)
## HTML 表格表头
HTML 表格的表头使用 ```<th>``` 标签进行定义。  
大多数浏览器会把表头显示为粗体居中的文本。  
实例：下面是一个带有表头的表格。
```angular2
<table border="1">
  <tr>
    <th>Header 1</th>
    <th>Header 2</th>
    <th>Header 3</th>
  </tr>
  <tr>
    <td>row 1, cell 1</td>
    <td>row 1, cell 2</td>
    <td>row 1, cell 3</td>
  </tr>
  <tr>
    <td>row 2, cell 1</td>
    <td>row 2, cell 2</td>
    <td>row 2, cell 3</td>
  </tr>
</table>
```
在浏览器中显示如下：  
![表](img/biao4.png)
## HTML 合并单元格  
HTML 合并单元格也称为表格的跨行跨列。  
rowspan 属性定义单元格应该横跨的行数，如 rowspan=2，表示横跨两行。  
colspan 属性定义单元格应该横跨的列数，如 colspan=4，表示横跨四列。  
实例1：下面是一个横跨两行的表格单元格。
```angular2
<table border="1">
  <tr>
    <td>First Name:</td>
    <td>Lucy</td>
  </tr>
  <tr>
    <td rowspan="2">Telephone:</td>
    <td>666 77 888</td>
  </tr>
  <tr>
    <td>666 77 889</td>
  </tr>
</table>
```
在浏览器中显示如下：  
![表](img/biao5.png)  
实例2：下面是一个横跨两列的表格单元格。
```angular2
<table border="1">
  <tr>
    <th>Month</th>
    <th>Savings</th>
  </tr>
  <tr>
    <td>January</td>
    <td>¥1000</td>
  </tr>
  <tr>
    <td>February</td>
    <td>¥800</td>
  </tr>
  <tr>
    <td colspan="2">Sum: ¥1800</td>
  </tr>
</table>
```
在浏览器中显示如下：  
![表](img/biao6.png)








