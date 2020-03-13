# 第一章 CSS基础
## 什么是 CSS?
+ CSS 指层叠样式表 (Cascading Style Sheets)
+ 样式定义如何显示 HTML 元素
+ 样式通常存储在样式表中
+ 把样式添加到 HTML 4.0 中，是为了解决内容与表现分离的问题
+ 外部样式表可以极大提高工作效率
+ 外部样式表通常存储在 CSS 文件中
+ 多个样式定义可层叠为一个
> 在学习CSS之前，你需要具备HTML的基本知识。  
> 如果你想学习HTML，可以先完成我们的HTML微课。
## 为什么使用CSS？
CSS允许您针对HTML元素应用特定的样式。  
CSS的主要好处在于，它允许你将样式与页面内容进行分离。  
仅使用HTML，样式将和页面内容格式混杂在一起，这样的页面将会变得难以维护。
>  所有的web页面样式都可以（也应该）从HTML文档中分离出来，建立成一个单独的CSS文件再进行引用。
## 内联 CSS
在web文档中直接插入一个CSS是内联样式的使用方法之一。使用内联样式，将CSS应用于单个元素。  
为了使用内联样式，将CSS属性直接添加到相关标签中。  
下面的例子展示了如何创建一个灰色背景和白色文本的段落：
```angular2
<p style="color:white; background-color:gray;">
    This is an example of inline styling. 
</p>
```
## 内部样式表
在HTML页面的标题部分将内部样式定义在<style>元素中  
例如：下列代码中的样式将作用在所有<p>段落中  
```angular2
<html>
   <head>
      <style>
      p {
         color:white;
         background-color:gray;
      }
      </style>
   </head>
   <body>
      <p>This is my first paragraph. </p>
      <p>This is my second paragraph. </p>
   </body>
</html>
```
## 外部引用CSS
通过这种方法将所有的CSS样式保存在同一个后缀名为.css的拓展文件中。    
然后通过html标签<link>在HTML页面的<head>部分将CSS文件引入。  
如下例子所示：
```angular2
<head>
   <link rel="stylesheet" href="example.css">
</head>
<body>
   <p>This is my first paragraph.</p>
   <p>This is my second paragraph. </p>
   <p>This is my third paragraph. </p>
</body>
```

