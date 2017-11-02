JS中的BOM对象
1.事件处理机制
```
事件源对象是指与事件相关的页面文档以及元素对象
事件的名称
属性	发生的场景
onload	当页面或图片加载完成时
onclick	当鼠标点击某个对象时
onchange	当用户改变域的内容时
onfoucs	当元素获得焦点时
onmouseover	当鼠标移动到元素上方时
onmouseout	当鼠标离开元素上方时
onkeypress	当键盘的键被按下时
onerror	当加载文档或图像时发生某个错误
。。。	。。。
```
2.事件处理机制方式
```
行内绑定
//第一种
<input  type=“button”  value  =  “确定”  onclick = “console.log(‘Say hello!’)">

//第二种
<input  type = “button”  value = “确定”  onclick = "show()">
<script>
	function  show(){
		console.log(“Say hello!”);
	}
</script>

动态绑定   //执行多个事件时会覆盖

<input  type = “button”  value = “确定”  id = “btn">
<script>
document.getElementById(“btn”).onclick =   function(){
		console.log(“Say hello!”);
	}
</script>

事件监听 //不会覆盖
<input  type = “button”  value = “确定”  id = “btn">
<script>
   document.getElementById(“btn”).
   addEventListener (“click”,function(){
		console.log(“Say hello!”);
	});
</script>

```
3.BOM可实现功能
```
弹出新的浏览器窗口
移动、关闭浏览器窗口以及调整窗口的大小
页面的前进、后退、刷新和重新加载
获取操作系统和浏览器的信息
```
4.window对象
```
window.open("adv.html",""," height=380,width=320,left=100,top=100

常用的方法
方法名称	    说      明
resizeBy( ) 把窗口的大小尺寸调整指定的像素         	
resizeTo( )	把窗口的大小尺寸调整到指定的宽度和高度
moveBy( )	把当前窗口移动指定的像素距离
moveTo( )	把窗口的左上角移动到指定的坐标
scrollBy( )	滚动指定的像素距离,内容必须大于窗口的尺寸
scrollTo( )	滚动到指定的坐标位置
setTimeout( )	在指定的毫秒数后调用函数或计算表达式
setInterval( )	按照指定的周期（以毫秒计）来调用函数或表达式
```
5.定时方法
```
setTimeout()
setTimeout("调用的函数",等待的毫秒数)

setInterval()
setInterval("调用的函数",间隔的毫秒数)

//如果要多次调用，使用setInterval()或者让disptime()自身再次调用setTimeout()
```
6.清除定时方法
```
clearTimeout()
clearTimeout(setTimeOut()返回的ID值)

var  myTime＝setTimeout("disptime() ", 1000 );
clearTimeout(myTime)；

clearInterval ()
clearInterval(setInterval()返回的ID值)

var  myTime＝setInterval("disptime() ", 1000 );
clearInterval(myTime)；

```






