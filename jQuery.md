jQuery
1.Javascript为何需要面向对象
```
Javascript程序中全局变量存在的问题
全局变量污染，影响程序运行结果
代码重用性差
```
2.Javascript类的实现方式
```
Object方式

Objecet是所有类的父类，可以使用Object表示其他类

函数方式

函数名作为类名，函数内部包含的属性和方法作为类成员
```
3.Javascript对象的创建 
```
字面量方式创建对象
构造函数方式创建对象

Javascript中可以采用简便的字面量方式创建对象
var obj = {		
	stuName:‘Tom’,		
	stuSex:‘男’,		
	stuAge:20,		
	sayHello:function(){		
		alert(“你好!”);		
	}	
}
//创建对象简便快捷，属性和值映射关系清晰
主要适用于一个实例对象的场合,缺乏封装性和重用


构造函数方式
function Human(name,age){     this.name=name;     this.age=age;
     this.show = function(){	
   	 alert(‘你好！我是’ + this.name);
      }
    ｝
//this表示当前作用域下的对象
不同作用域下this表示的对象不同
在函数中指向的是window
在方法中指向的是调用该方法的对象
```
4.对象类型的判断
```
typeof函数
返回对象的具体类型
instanceof函数
判断对象是否是某种类型的实例
```
5.构造方式总结
```
构造方法在创建对象时发挥作用，不创建对象时和普通方法相同，
构造方法名首字母大写，通过new关键字创建实例对象
构造方法中不需要创建对象，也不用返回，依靠this关键字实现属性的设置
构造方法的对象是独立存储的，缺少共享，内存空间消耗较大
```




