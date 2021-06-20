# html总结

HTML是超文本标记语言（HyperText Markup Language）的缩写。我们用 HTML 来构建 Web 页面即所谓的网页。HTML 是构成 Web 世界的一砖一瓦。它定义了网页内容的含义和结构。除 HTML 以外的其它技术则通常用来描述一个网页的表现与展示效果（如 CSS），或功能与行为（如 JavaScript）。HTML 不是一门编程语言，而是一种用于定义内容结构的标记语言。在浏览器中看到的任何网页背后都是一个 HTML 文档，只要在网页上点击鼠标右键->查看源代码（用控制台工具也可）就可看到。



## html相关说明

### 注释

为了将一段 HTML 中的内容置为注释，你需要将其用特殊的记号<!--  -->

在 code 软件中，输入Ctrl + /即可快捷的进行注释！



### 空元素 

一般来说，元素都拥有开始标签，内容，结束标签。但有一些元素只有一个开始标签，通常用来在此元素所在位置插入/嵌入一些东西，如<mark>br, hr, input, img, a</mark>等等。我们称其为空元素。

  

### 元素的属性

元素是可以有相关属性的。属性包含元素的额外信息，这些信息不会在浏览器中显示出来。

<pre>一个属性必须包含如下内容：
    1.一个空格，在属性和元素名称之间。(如果已经有一个或多个属性，就与前一个属性之间有一个空格。)
    2.属性名称，后面跟着一个 = 号。
    3.一个属性值，由一对引号 "" 引起来。</pre>  
### 题

<p>HTML 提供了从大到小6级标题
        <pre>
    在页面中，标题非常重要：
    1.搜索引擎用标题来索引页面的内容
    2.用户也习惯以标题进行主要内容浏览，以决定是否查看该页面

            </pre>

### 超链接a

<pre>
没有超链接就没有万维网（World Wide Web）。基本上，我们可以把任何东西加上超链接，不过常用的是文本、图片等。
说明：
    href即为要跳转去的地址 URL（Uniform Resorce Locator)
    target属性为_blank表示在新的页面打开超链接（默认是在当前页面打开即_self）
    超链接标签包含的内容（当前为文字"百度一下"）即为显示在页面上供用户点击的
        </pre>
### 锚点

<pre>          
锚点，也称为书签，用于标记页面的某个元素或位置。通过锚点，我们可以轻易的在长页面内实现跳转。
先使用id属性生成某元素的锚点，然后再使用超链接指向该锚点即可。
注意：
     1.元素的id值必须是唯一的，也即页面不能再有其它元素的id值为C4
     2.超链接中的地址需要有#符号   
        </pre>
### 图片及文件路径

说明：

  1.src属性为要显示图片文件的位置 URL，即图片文件的路径

  2.alt属性当获取图片出现问题时显示的文字（占位符）

  3.可为图片指定高宽度，但不建议（可能导致图片变形）  

特别注意图片的路径，如果图片路径不对，那么不能正确插入我们所需要的图片

  

### 列表

列表分为无序列表和有序列表 

无序列表默认使用**实心圆点**作为每项的标志，其它的标志可以是空心圆`circle`，实心方块`square`以及不出现标志。

有序列表默认使用**数字**作为每项的标志，其它的标志可以是大写字母`A`，小写字母`a`，罗马字母`i`等



### 表单

表单用来填一些问卷之类的 东西。

  

### 其他

<pre>
HTML 的元素可以以称为区块 或 内联的方式进行显示。
区块元素在浏览器显示时，通常会以新行来开始（和结束）。
内联元素相反，他们总是一个接一个进行显示，不会新起一行。
如果你想在网页中展示一首诗或一些特别格式的文本，那么请使用pre标签。
有时候需要特定表示一些字符则需要使用字符实体，如br
          </pre>