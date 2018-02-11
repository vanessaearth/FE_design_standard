# head标签中添加按设备缩放
~~~
<meta name="viewport" content="width=device-width, initial-scale=1, maximum-scale=1,user-scalable=no">
~~~
# 移动端css文件使用rem单位替换px
~~~
@media only screen and (max-width: 319px){html{font-size: 42.53px;} }
@media only screen and (min-width: 320px){html{font-size: 42.67px;} }
@media only screen and (min-width: 360px){html{font-size: 48px;} }
@media only screen and (min-width: 375px){html{font-size: 50px;} }
@media only screen and (min-width: 384px){html{font-size: 51.2px;} }
@media only screen and (min-width: 414px){html{font-size: 55.2px;} }
@media only screen and (min-width: 540px){html{font-size: 72px;} }
@media only screen and (min-width: 640px){html{font-size: 85.33px;} }
@media only screen and (min-width: 750px){html{font-size: 100px;} }

.box{
    width: 0.15rem;
    height: 0.15rem;
    background: greenyellow;
    font-size: 2rem;
}
<div class="box">这是测试div</div>
~~~
#### 设计图要求： width：750px

 根据设计图标准的像素大小，对应的除以100，得到当前box的大小；
 例如：标注宽100px，高120px
 ```
 .box{
   widrh: 1rem;
   height: 1.2rem;
   }
```