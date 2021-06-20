#                                CSS总结

## 1. 何为css

**CSS**是级联样式表（Cascading Style Sheets）的缩写。HTML 用于撰写页面的内容，而 CSS 将决定这些内容该如何在屏幕上呈现。网页的内容是由 HTML的元素构建的，这些元素如何呈现，涉及许多方面，如整个页面的布局，元素的位置、距离、颜色、大小、是否显示、是否浮动、透明度等等。要想一个网页变得好看，css必不可少。

## 2. CSS语法

一条CSS样式规则由两个主要的部分构成：选择器，以`{}`包裹的一条或多条声明:

<pre>
这条规则表明，页面中所有的一级标题都显示为蓝色，字体大小为12像数。
说明：
    选择器是您需要改变样式的对象（上图的规则就一级标题生效）。
    每条声明由一个属性和一个值组成。（无论是一条或多条声明，都需要用{}包裹，且声明用;分割）
    属性（property）是您希望设置的样式属性（style attribute）。每个属性有一个值。属性和值被冒号分开。    
</pre>

### 2.1选择器

一个页面上的元素众多，选择器就用于在页面中找到/选择需要应用这个样式的对象。
除我们前示的元素选择器外，还有`id`和`class`选择器。其中`class`选择器使用非常普遍。

#### 2.11 id选择器

id选择器前面有#号

#### 2.12 class选择器

class选择器前有 . 号，class的值可以是多个，也可以重复，因此class选择器非常普遍。



## 3. CSS如何生效

css样式表有三种，为外部样式表，内部样式表，内联样式。外部样式表需要新创一个css文件，内部样式表放在html里面，但是需要引入style标签；内联样式表就是直接把样式规则直接写到要应用的元素中，一般很少用。样式定义离元素的距离近，哪个就生效。



## 4. 颜色，尺寸，对齐

颜色在网页中的重要性不言而喻。
我们可以采用颜色名称也可以使用颜色RGB16进制值，来设定前景或背景的颜色。

我们可以用 `height` 和 `width` 设定元素内容占据的尺寸。常见的尺寸单位有：像数 `px`，百分比 `%`等。

对于**元素中的文本**，我们可以简单的设置`text-align`属性为`left, center, right`即可（显然缺省的是左对齐），上例中已有相关的应用。



## 5. 盒子模型、边框与边距

一个html元素可以看作一个盒子，可以使得我们的网页布局变得更加大气可观。边距使得文章不紧凑，使人赏心悦目。



## 6.定位

<pre>
   position属性用于对元素进行定位。该属性有以下一些值：

    static 静态
    relative 相对
    fixed 固定
    absolute 绝对

</pre>



## 7. 溢出

当元素内容超过其指定的区域时，我们通过溢出`overflow`属性来处理这些溢出的部分。
溢出属性有一下几个值：

- visible 默认值，溢出部分不被裁剪，在区域外面显示
- hidden 裁剪溢出部分且不可见
- scroll 裁剪溢出部分，但提供上下和左右滚动条供显示
- auto 裁剪溢出部分，视情况提供滚动条



## 8. 浮动

我们可以设置`float`属性让某元素水平方向上向左或右进行移动，其周围的元素也会重新排列。
我们常用这种样式来使图像和文本进行合理布局，如我们希望有以下的效果

 

## 9. 不透明度

我们可以用`opacity`对任何元素（不过常用于图片）设置不透明度。
值在`[0.0～`1.0]之间，值越低，透明度越高



### 10. 组合选择器

组合选择器配合使用，能够得到简洁精确的结果



### 11. 伪类和伪元素

伪类（pseudo-class）或伪元素（pseudo-element）用于定义元素的某种特定的状态或位置等。
比如我们可能有这样的需求：

- 鼠标移到某元素上变换背景颜色
- 超链接访问前后访问后样式不同
- 离开必须填写的输入框时出现红色的外框进行警示
- 保证段落的第一行加粗，其它正常
