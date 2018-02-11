## 1.小图标用css精灵合并
小图标合并到一个文件中，以减少请求数，用定位取到需要的图标
![](images/vip.png)
~~~
<i class="icon-vip vip-1"></i>
<i class="icon-vip vip-2"></i>
<i class="icon-vip vip-3"></i>
<i class="icon-vip vip-4"></i>
.icon-vip{
	display:inline-block;
	width:20px;
    height:20px;
    background:url(../images/vip.png) no-repeat 0 0;
}
.vip-1{
	background-position:0 0;
}
.vip-2{
	background-position:0 -20px;
}
.vip-3{
	background-position:0 -40px;
}
.vip-4
	background-position:0 -60px;
}
~~~