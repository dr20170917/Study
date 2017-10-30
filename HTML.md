HTML知识点
1.锚点
       
    a.锚记标签用于使用户“跳”到文档的某个部分 
      HTML 的 NAME 属性用于创建锚标记       
      为达到这种跳转效果，请在 HREF参数中使用该标记
    b.target属性
    使用target属性，可以定义被链接的文档在何处显示。
    target=_blank页面在新窗口打开
    target=self在当前窗口打开新页面

2.字符格式化标签
 
     a.粗体、斜体、下划线、上标、下标等。
     b.<b></b>、<i></i>、<u></u>、        <sub></sub>、<sup></sup>
3.无序列表、有序列表、自定义列表
     
     a.<ul><li></li></ul>
     b.<ol><li></li></ol>
     c.<dl><dt>小标题<dd>文本</dd></dt></dl>
     
4.特殊字符

    a.大于号（>）&gt
    b.小于号（<）&lt
    c.引号（''）&quot
    d.&号&amp
    
5.水平线
   
    hr标签
6.多媒体元素
```
利用<marquee>标签可以让文字在网页上动态滚动。
方向：<marquee direction=#>。 #可以是：left、right
方式：<marquee behavior=#>。 #可以是scroll、slide、alternate
循环：<marquee loop=#>。#代表次数 
速度：<scrollamount=#>。指滚动速度。
延时：<scrolldelay=#>。指文字滚动间隔。scrolldelay值是毫秒。
使用bgsound标签来给网页设置背景音乐。
<bgsound src=”jy001.mid” loop=3> 	 
```
7.总结
```
标题级标签使用<H1>…<H6>
段落标签使用<P align＝“对齐方式”>…</P>
无序列表使用<UL>标签,有序列表使用<OL>标签
插入图片：<img src=? Align =?>
插入横线：<hr color=?  Size=? Width=? Align=?>

```
8.表格、表单
```
<HTML>
<HEAD>
<TITLE>使用表格</TITLE>
</HEAD>
<BODY>
<TABLE BORDER = 2 cellspacing="1" >
<CAPTION align=top>学员档案信息</CAPTION>
 <TR>
   <TH COLSPAN = 3>姓名</TH>
   <TH>性别</TH>
   <TH>分数</TH>
 </TR>
 <TR>
   <TD ROWSPAN = 3>姓名</TD>
   <TD>性别</TD>
   <TD>分数</TD>
 </TR>
 <TR>
  <TD>Robert</TD>
  <TD>M</TD>
  <TD>80</TD>
 </TR>
 .......
</TABLE>
</BODY>
</HTML>

<TABLE>代表表格的开始，border=2表示边框尺寸为2

<TR>表示行，这是表格的第一行，有三列数据，<TD>代表列 

<CAPTION>表示表格标题

<TH>表示行或列标题，粗体显示 

COLSPAN=“n” 属性表示跨多少列

ROWSPAN=“n” 属性表示跨多少行

设置单元格间距：cellspacing 
设置单元格填充距离：cellpadding 
可以利用cellspacing和背景颜色设置表格为细线表格

```
9.表单简介
```
最常见的表单主要包括文本框、单选按钮、复选框、按钮等，如下图所示，是一个常见的注册页面，它包含了文本框、单选按钮、复选框、按钮等表单内容。

<form name="表单名" method="传送方式" action="表单处理程序 "> 
action指定提交后由服务器上哪个处理程序处理
method指定向服务器提交的方法:一般为post或get方法, post方法比较安全

按表单元素的填写方式可以将表单分为输入类控件和菜单列表类控件
输入类控件一般以input标记开始，说明这一表单元素需要用户的输入；
菜单列表类以select开始，表示用户需要选择
```
10.input所包含的元素类型
```
type值	说明
text	文本字段
password	密码域，用户在输入时不显示具体内容，以*代替
radio	单选按钮
checkbox	复选框
button	普通按钮
submit	提交按钮
reset	重置按钮
hidden	隐藏域
file	文件域
```
11.select
```
<select name="content" size="3" multiple>      
<option value="m1">体育栏目</option>      
<option value="m2">科技栏目</option>      
<option value="m3">新闻栏目</option>    
<option value="m4">汽车栏目</option>
<option value="m5">房产栏目</option>
</select>

Multiple属性表示在列表
中可以选择多项 

```
12.textarea
```
<textarea name="info" cols="35" rows="7">请将意见输入此区域
</textarea> 
cols属性设置区域的宽度
rows设置文本区域包含的行数

```
 
    






