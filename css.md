CSS
1.CSS是Cascading StyleSheet的缩写，
可以翻译为“层叠样式表”或“级联样式表”，即“样式表”。
2.CSS样式表的功能一般可以归纳为以下几点：
```
灵活控制网页中文字的字体、颜色、大小、间距、风格及位置。
随意设置一个文本块的行高、缩进，并可以为其加入三维效果的边框。
更方便地为网页中的任何元素设置不同的背景颜色和背景图片。
精确控制网页中各元素的位置
可以与脚本语言相结合，使网页中的元素产生各种动态效果。
```
3.CSS的基本语法 
选择器 { 样式属性：属性值 ; 样式属性：取值 ; }

4.样式表的常用属性
```
属性	    CSS名称	          说明
字体属性	font-family	  设置或检索文本的字体
            Font-size	  设置或检索文本字体的大小
            Font-style 设置或检索文本的字体样式，即字体风格，主要设置字体是否为斜体。取值范围：normal  |  italic  |  oblique
            Font-weight	用于设置字体的粗细，取值范围：
Normal  |  bold  |  bolder  |  lighter  |  number 100-900
Text-decoration	None | underline |line-through |blink
Text-underline-positon	above
Letter-spacing	字符间距
Word-spacing	单词间距
文本属性	Text-align

Line-height	设置文本的对齐方式，如：左对齐、右对齐、居中对齐、两端对齐/垂直居中
Text-indent	设置文本第一行的缩进量，取值可以是一个长度或一个百分比
Vertical-align	设置文本的纵向位置(适用单元格)

边框属性	Border-style	设置边框的样式
            Border-width	设置边框的宽度
            Border-color	设置边框的颜色
            Border-left  	设置左边框的属性

外边框      outline	outline	
            outline-width	设置元素的高度
            outline-color	设置边框的颜色
            outline-style	设置边框的样式
```
5.表格样式
```
border-collapse	separate	默认值。边框会被分开。不会忽略        border-spacing 和 empty-cells 属性。
collapse	如果可能，边框会合并为一个单一的边框。会忽略 border-spacing 和 empty-cells 属性。
border-spacing	Length/length	规定相邻单元的边框之间的距离。使用 px、cm 等单位。不允许使用负值。如果定义一个 length 参数，那么定义的是水平和垂直间距。如果定义两个 length 参数，那么第一个设置水平间距，而第二个设置垂直间距。
caption-side	Top/bottom	顶/底
Empty-cells	Hide/show	隐藏/显示
```
6.样式表的常用属性
```
属性	CSS名称	说明
颜色及背景属性	Background
background  background-color || background-image || background-repeat || background-attachment || background-position 

Background-color	设置背景颜色 
rgba(r,g,b,0.4) 设置背景透明度
background-image	设置元素的背景图象
background-repeat 	repeat | no-repeat | repeat-x | repeat-y 
background-position :	length || length   position || position 

Background:	Transparent 背景透明

Display属性
block	块
inline	行内
Inline-block	行内块
List-item	列表项
尺寸及定位属性
Width	设置元素的宽度
Height	设置元素的高度
Left	定位元素的左边距
Top	定位元素的顶边距
Position	设定浏览器如何来定位元素，
absolute表示绝对定位，需要同时使用left、right、top、bottom等属性进行绝对定位
z-index	设置层的层叠先后顺序和覆盖关系
```
7.定位
```
CSS 有三种基本的定位机制：普通流、浮动和绝对定位。
值描述
absolute
生成绝对定位的元素，相对于static定位以外的第一个父元素进行定位。元素的位置通过 "left", "top", "right" 以及"bottom"属性进行规定。
         
fixed
生成绝对定位的元素，相对于浏览器窗口进行定位。
元素的位置通过 "left", "top", "right" 以及 "bottom" 属性进行规定。

relative
生成相对定位的元素，相对于其正常位置进行定位。
因此，"left:20" 会向元素的 LEFT 位置添加 20 像素。
static 默认值。没有定位，元素出现在正常的流中（忽略 top, bottom, left, right
或者 z-index 声明）。

```
8.根据样式代码的位置，分为三类：
```
行内样式
内嵌样式
外部样式

根据选择器的不同，内嵌样式又分为：
HTML 选择器
CLASS 类选择器
ID 选择器
选择多个样式

外部样式
根据样式文件与网页的关联方式又分为：
链接（LINK ）外部样式表
导入（import）外部样式表
<LINK   rel = “stylesheet”    type = ”text/css”    href = ”样式表文件.css” >

<STYLE TYPE="text/css">
@ import  样式表文件.css;
</STYLE>
```


