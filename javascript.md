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
splice( )	删除数组中的部分元素//返回的是删除的数字

  <script>
    var num=[1,2,3,4,5,6]
    console.log(num.splice(2, 1));
  </script>
  //输出的结果是3.
  
sort( )	对数组排序//不是按照大小排序
push( )	向数组末尾添加一个或更多 元素
pop( )	从数组尾部删除并返回一个元素
shift( )	从数组头部删除并返回一个元素
unshift( )	从数组头部添加一个或更多元素
```
21.String是Javascript提供的描述字符串的对象
```
length	获取字符串的字符长度
charAt()	获取字符串中指定位置的字符
concat()	把一个或多个值连接到字符串上
indexOf()	获取指定字符在串中的初始索引位置
lastIndexOf()	获取指定字符在串中的最后索引位置
split()	把字符串按指定字符分割成数组
substr()	截取字符串//从截取的位置返回数组内容
var str='hello javascript!';
console.log(str.substr(3));
返回lo javascript!

slice()	截取字符串
toUpperCase()	把字符串转换成大写
```
22.在字符串中slice（）、substring（）和substr（）区别
```
stringObject.substring(start,stop) 用于提取字符串中介于两个指定下标之间的字符。
start必需。一个非负的整数，规定要提取的子串的第一个字符在 stringObject 中的位置。
stop可选。一个非负的整数，比要提取的子串的最后一个字符在 stringObject 中的位置多 1。如果省略该参数，那么返回的子串会一直到字符串的结尾。
start从0开始 到stop(不包含stop)结束 不接受负的参数。

stringObject.substr(start,length)可在字符串中抽取从start下标开始的指定数目的字符
start 必需。要抽取的子串的起始下标。必须是数值。如果是负数，那么该参数声明从字符串的尾部开始算起的位置。也就是说，-1 指字符串中最后一个字符，-2 指倒数第二个字符，以此类推。
length 可选。子串中的字符数。必须是数值。如果省略了该参数，那么返回从 stringObject 的开始位置到结尾的字串。

stringObject.slice(start,end)提取字符串的某个部分，并以新的字符串返回被提取的部分
start 要抽取的片断的起始下标。如果是负数，则该参数规定的是从字符串的尾部开始算起的位置。也就是说，-1 指字符串的最后一个字符，-2 指倒数第二个字符，以此类推。
end 紧接着要抽取的片段的结尾的下标。若未指定此参数，则要提取的子串包括 start 到原字符串结尾的字符串。如果该参数是负数，那么它规定的是从字符串的尾部开始算起的位置。
返回新的字符串包括字符串 stringObject 从 start 开始（包括 start）到 end 结束（不包括 end）为止的所有字符
```
23.Math对象
```
Math是用于执行数学运算的对象，提供了大量的数学运算函数

Math.PI	获取圆周率π
Math.round()	进行四舍五入取整运算
Math.ceil()	进行小数进位运算
Math.floor()	进行取整运算
Math.random()	获取随机数 [ 0~1）
Math.pow()	进行指数运算
Math.abs()	进行绝对值运算
```
24.Date是JS提供的关于日期的内置对象
```
var date = new Date(参数);
没有参数时获取当前系统时间
有参数时获取参数指定的时间，参数必须
符合时间格式
```
25.常用日期对象的方法
```
getDate()	获取天数
getDay()	获取星期数
getMonth()	获取月份
getFullYear()	获取完整的年份
getHours()	获取小时数
getMinutes()	获取分钟数
getSecond()	获取秒数
getMilliseconds()	获取毫秒数
getTime()	获取累计毫秒数，从1970-1-1开始计算
toLocaleString()	获取完整的日期和事件字符串
```
26.arguments对象针对函数的参数进行了封装
常见和属性
length：参数的个数
callee:返回当前执行的函数，用于递归
