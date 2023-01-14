# 知识点

符合选择器、背景样式

## 题目1（加强训练）

​ 页面上有购物车标签，该标签点击后会跳转到购物车页面，所以必须使用a标签来实现；并且该标签在鼠标经过的时候背景图会发生更替。请使用css和HTML代码实现以上效果。

### 训练目标

能够使用背景样式设置背景图。

### 训练提示

1、使用background-image样式设置背景图片。

2、当鼠标经过a标签的时候更换背景图片。

3、a标签无法设置宽高，需要先转换显示模式再设置宽高

### 参考方案

使用display转换显示模式，使用background-image来设置背景图

### 操作步骤

1、创建a标签

2、设置a标签的显示模式为块或者行内块

3、设置a标签的宽高，宽高等于图片的宽高

4、设置a标签的背景样式，使用background-image来引入背景图片

5、当鼠标经过a标签的时候，更换背景图

### 参考答案

HTML代码

```html
<a href="#"></a>
```

CSS代码

~~~css
a {
    display: block;
    width: 67px;
    height: 31px;
    background: url(shopcar_01.png) no-repeat;
}

a:hover {
    background-image: url(shopcar_02.png);
}
~~~

## 题目2（加强训练）

在页面中，输入框使用功能input标签来实现，当鼠标点击输入框的时候，输入框会获得焦点，同时为了给用户以提示，通常会更换输入框的部分样式，现在需要让输入框被点击获得焦点之后修改背景图片。如下图所示：

![](images\百度输入框.gif)

### 训练目标

能够使用焦点伪类来实现获得焦点的样式制作。

### 训练提示

1、如何让“相机”图片在输入框的右侧居中？

2、如何设置获取焦点的样式？

### 参考方案

使用while循环语句完成

### 操作步骤

1、使用input标签创建一个输入框

2、设置宽高为535px宽，40px高

3、通过背景样式设置背景图，并且设置背景不平铺，背景图定位在靠右侧垂直居中的位置

4、通过focus来设置获得焦点样式

### 参考答案

HTML代码

```html
<input type="text">
```

CSS代码

```css
input {
    width: 535px;
    height: 40px;
    background: url(camera_01.png) no-repeat 500px center;
}

input:focus {
    width: 535px;
    height: 40px;
    background: url(camera_02.png) no-repeat 500px center;
}
```

## 题目3（综合案例）

在网页的顶部，通常会有导航栏来引导用户进入不同的功能区域，当点击不同的导航部分的时候会跳转到不同的页面中。所以往往导航栏需要使用功能a标签来完成。现在请使用HTML与CSS来实现以下所示导航栏：

![](images\导航栏.gif)

### 训练目标

能够转换显示模式，能够单行文本垂直居中，能够让文本水平居中，能够使用链接伪类。

### 训练提示

1、如何让文字水平居中、垂直居中？

2、设置鼠标经过的样式？

### 参考答案

HTML代码

```html
<a href="#">新闻</a>
<a href="#">体育</a>
<a href="#">汽车</a>
<a href="#">娱乐</a>
```

CSS代码

```css
a {
    display: inline-block;
    width: 100px;
    height: 40px;
    line-height: 40px;
    background-color: pink;
    text-align: center;
    color: #fff;
    text-decoration: none;
    font-weight: 700;
}

a:hover {
    background-color: orange;
    color: black;
}
```

