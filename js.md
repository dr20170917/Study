JavaScript

1.JavaScript的基本结构
```
<script type=“text/javascript”>
    JavaScript 语句;
</script >
```
可以包含在文档中的任何地方

2.外部JS文件
```
<script src="hello.js" language="javascript"></script>
```
3.直接在HTML标签中
```
<a href="javascript:alert('hello js!')">click me!</a>
```
4.常用的输入/输出
```
alert()
prompt()
console
console.log()	控制台输出普通输出语句
console.warn() 	控制台警示
console.error();	错误提示
```
5.变量是一个标识符，在程序运行过程中用于保存临时数据
6.变量
```
先声明变量再赋值
var   width;
width = 5;

同时声明和赋值变量
var catName= “皮皮”;
var x, y, z = 10;

不声明直接赋值
width=5;
//变量可以不经声明而直接使用，但这种方法很容易出错，也很难查找排错，不推荐使用。
```
7.变量命名语法规定
必须是字母、数字、下划线和$组成
首字母不能是数字
不能使用Javascript保留字
命名区分大小写

8.数据类型
```
undefined
null
number
boolean
string
object
```
9.typeof检测变量的返回类型值
```
typeof运算符返回值如下：
undefined：变量被声明后，但未被赋值
string：用单引号或双引号来声明的字符串
boolean：布尔值
number：整数或浮点数
object：javascript中的对象、数组和null
```
10.运算符具有优先级，通过（）可以改变优先级
逻辑运算符的优先级！ > && > ||

11.+连字符

12.if条件语句
```
基本条件语句
多重条件语句
嵌套条件语句
```
13.switch多分支语句
```
switch (表达式)
{         case 常量1 : 
 	   JavaScript语句1;
	   break;
 	case 常量2 : 
 	   JavaScript语句2;
 	   break;
 	...
 	default : 
                 JavaScript语句3;    
}
```
14.for、while循环语句
```
or(初始化;  条件;  增量)
 {
    JavaScript代码; }

while(条件)
 {
 JavaScript代码;
}
```
15.循环中断
```
break//退出整个循环
continue//退出当次循环
```
16.程序调试
```
alert()方法
浏览器开发工具
单步进入
单步跳过
单步退出
```
17.常用系统函数
```
parseInt ("字符串")
将字符串转换为整型数字 
如: parseInt ("86")将字符串“86”转换为整型值86
parseFloat("字符串")
将字符串转换为浮点型数字 
如: parseFloat("34.45")将字符串“34.45”转换为浮点值34.45
isNaN()
用于检查其参数是否是非数字
```
18.作用域
```
全局作用域：在代码的任何位置都可以访问
最外层的函数,<script>内部定义
最外层函数外定义的变量,<script>内部定义
隐式全局变量
局部作用域：在指定的代码段范围中可以访问
函数内部定义的变量
```
19.Javascript提供了大量的内置对象
```
Array
String
Math
Date
Arguments 
RegExp
```
20.数组访
```
数组名[下标]

数组的常用属性和方法
length	设置或返回数组中元素的数目
join( )	把数组的所有元素放入一个字符串，通过一个的分隔符进行分隔
splice( )	删除数组中的部分元素
sort( )	对数组排序//不是按照大小排序
push( )	向数组末尾添加一个或更多 元素
pop( )	从数组尾部删除并返回一个元素
shift( )	从数组头部删除并返回一个元素
unshift( )	从数组头部添加一个或更多元素
```
