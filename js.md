## 1.统一立即执行函数写法
~~~
(function(){
...
}())
~~~
## 2.变量会提前，方法内首行声明变量
 
## 3.判断使用相等用===而不是==
## 4.切勿在循环中创建函数
## 5.this关键字
在对象构造器，方法和闭包中使用this，
this可以指向全局对象
可以指向DOM树种某一节点
可以指向新创建的对象（构造器中）
可以指向一些对象（函数被call()和apply()执行调用时）

## 6.数组迭代用Array.forEach(不可中断)，需要中断可以用Array.every()

## 7.用if/else 代替switch（switch难控制）
## 8.对象声明用{}和,数组声明用[]
~~~
var arr=[];
var obj={};
~~~
## 9.静止修改已有对象原型Array.prototype和Object.prototype

## 10.简单情况下用三元条件语句代替if/else
~~~
if(name===null){
	name='Tom'
}
name===null ? name='tom' : name
~~~
