## 使用语义化的命名方式,用中划线(-)链接,eg:icon-play{}

## 1.尽可能精确选择
如使用子选择器
~~~
.box > title{ color: #f60 }    而不是    .box   title{ color: #f60 }
~~~
## 2.值是0，不用加单位
~~~
margin: 0      而不是   margin: 0px
~~~
## 3.颜色值用小写，能用三位不用6位
~~~
color: #f60   而不是   color: #ff6600
~~~
## 4.声明顺序
####  1. 表示结构的属性
~~~
   display
   position left right top bottom
   overflow float clear
   width height margin padding border
   ~~~
#### 2.表示显示的属性
~~~  
   background  
   font  
   text
~~~
## 5.多个选择器隔行显示
~~~
a:hover,
a:active{
}

h1,
h2,
h3{
	font-weight: 700
}
~~~
## 6.每个属性换行显示
~~~
.username{
	width: 100px;
    height: 100px;
}
~~~

## 7.属性值和冒号之间空一格
~~~
width: 100px；
~~~
## 8.url不要带引号
~~~
.user-photo{
	background: url(../images/user.png) no-repeat 0 0;
}
~~~
## 9.选择器嵌套顺序scss
1. 自己属性
2. 伪类选择器(:first-letter,first-child,:hover,:active 等等)
3. 伪类元素（:before :after）
4. 属性样式（.select  .active）
5. 媒体查询
6. 子选择器
~~~
a{
	color: #f60;
    &:first-child{
    	color: #ff0;
    }
    &:before{
    	content: '',
    }
    .select{
    }
    @media screen and( min-wid: 640px) {
    	color: #333;
    }
    >span{
    	font-size:20px;
    }
}
~~~

