# 壹、html,css

## 一、万维网（World Wide Web）

现在多译作互联网等的领域。

`web的三个表现形式：超文本、超媒体、超文本传输协议（https)*`

## 二、网站

（网站是网页的集合）在万维网的基础上通过html等工具制作的网页的集合。

## 三、网页

网页是网站的基本元素。主要使用html等工具来显示特定内容。

## 四、创建一个网页文件

`文档类型的文件更改它的后缀名为.html`

## 五、静态网页和动态网页

动态网页中的数据来自于数据库

## 六、html的文档结构hyper text MarkUp language 超文本标记语言

1.  英文状态下的 ！+tab     html:5+tab    [h5]

   2.html:4s [h4->4.01]

### （一）DOCTYPE：声明文档类型及版本号

### （二）head：主要放置和页面相关的一系列设置

1.编码格式：<meta charset="UTF-8">

UTF-8又称万国码     gb2312 

2.文档标题 ：<title>Document</title>

3.页面的**样式**

4.文档logo的设置

5.关键字

**在html中插入logo图片

<link rel="icon" type="image/png" sizes="16x16" href="/logo-16.png">

`<link rel="icon" href="favicon.ico(img url)" type="image/x-icon">`

<link rel="shortcut icon" href="favicon.ico" type="image/x-icon">

## （三）、body

## 七、html语法

1.标签：用尖括号括起来的，结束的标识必须是/

  `注意：*DOCTYPE不是标签，主要是用于声明文档类型及版本号`

2.属性：必须在开始标签中，而且和标签名用空格隔开，多个属性时用空格隔开。

3.元素：内容以及开始、结束标签

## 八、标签

 h1 +tab       h1*6+tab

<body>

```html
<!--标题标签-->
<h1></h1>
<h5></h5>
<!--段落标签-->
<p></p>
<span></span>
<i></i>
<em></em>
<b></b>
<strong></strong>
图片
<img src="" alt="" title="鼠标移入以后的提示信息">
<!-- <img src="3.jpg" alt="" title="查看此图片"> -->
	<a href="http://www.baidu.com:8080/list/html?a=content&&pass=2233#main">百度</a>
	         协议       域名     端口号 文件路径   查询的字符串           锚链接
```

</body>

注释标签

1.ctrl+/    
2.提高代码可读性；停止代码的执行

a标签常见的表现形式：
1.普通链接
2.空链接实现页面刷新功能 <a href="">刷新</a>
3.实现资料下载（压缩包）<a href="王彤彤.zip">下载</a>
4.实现锚链接[本页面实现链接]<a href="#answer">问题答案</a> <br>
 <br>
 <br>  <a href="" name="answer">这就是问题答案</a>

## 九、路径

相对路径

1.当前文件和目标文件在同级目录下，直接找

2.目标文件在同级目录下，另一个文件夹里，先找文件夹，再找目标文件。

3.不在同级目录下，先跳出至同级目录再进行查找。 ../代表退出一次

绝对路径：本地的，远程的

## 十、网页有三部分组成：

1.结构层 （html)

2.表现层（css）

3.行为层（javascript）

组成元素：图片 文字超链接 视频 音频

## 十一、css（*Cascading Style Sheets）层叠样式表

### 1.css语法

选中元素{

样式1;

样式2;

........

}

### 2.选择器 

​    1）标签选择器    .标签名{样式}    div   body  a

​     2) 类名选择器     .类名{样式}    

​     3)  id选择器：    #id名{样式1}

​    4）后代选择器:  父类 子类{样式1}   ul  li     .one .two

​    5）通用选择器   *{样式1}

​    6）群组选择器：.one , .two

​    7）交叉选择器     ul.one        .one .two

​    8) UI伪类选择器：给选中的元素设置某个状态下的效果

​         ：hover 鼠标移入状态      :link  :active  :visited

​    9）子选择器    div>a     .one>.two

   10)  同级选择器    div+p 紧挨着    div-p

   11）:nth-child( )  :first-child   :last-child    :nth-last-child()  :only-child   相对于父元素

​      :nth-of-type( )   :first-of-type   :last-of-type   :nth-last-of-type( )   :only--of-type  同类型里的选

​              :nth-child(2n-1 ){   }  奇数

   12）属性选择器  [date ]

​     	[date=a]

​	[date^=aa]

​	[ date$=aa]

​	[date*=aa]

   13)  :before  :after

   14）:checked

   15）:targer跳转的地址   :root

###  3.选择器的优先级问题

1）优先级一样时，就近原则

2）标签选择器优先级 1

​     类名选择器优先级 10

​     id选择器优先级      100

​     后代选择器优先级     依次累加

​     通用选择器优先级            最低

### 4.css特性：叠加特性，继承特性（文字、文本属性）

（一）、字体 文本样式

.title2{

```css
/*字体大小*/
font-size: 24px;
/*文字颜色*/
color: #2df;  十六进制
color: rgb(0, 0, 0);  rgb模式
color: red;  预定义模式
color: hsl(120, 30%, 30%); 工业的 色相（0-255）  饱和度%    亮度%
/*字体*/
font-family:"微软雅黑"，"苹方"，"宋体","黑体"；
/*字体粗细*/
font-weight: bold;
/*字体样式*/
font-style: normal;
```


```css
/*文本样式*/
text-decoration-line:  underline;
text-decoration-color: blue;
text-decoration-style: solid;
text-decoration:line-through 贯穿线
/*文本垂直居中*/
line-height: 50px;
/*文本水平居中*/
text-align: center;
/*字间距*/
letter-spacing: 20px;
/*首行缩进*/
text-indent: 48px;取决于字大小
word-break
letter-spacing
vertical-align
```

}

input独有：	

```css
input:focus{
	outline: none;
}
```


（二）、文本两端对齐

<head>

```html
<meta charset="UTF-8">
<title>文本属性</title>
<style>
.box{
	background-color: green;
	text-align:justify ;
}
.box i{
	display: inline-block;
	width: 100%;
	font-size:0 ;
	line-height: 0;
}
.box span{
	display: inline-block;
}
</style>
```

</head>
<body>

```html
<h1 class="box">
	<span>文本</span>
	<span>文本</span>
	<span>文本</span>
	<i></i>
</h1>
```

</body>

（三）、对文字溢出的处理

.box1{

```css
	width: 60px;
	height: 50px;
	background-color:pink;
	word-break: break-all;/*对英文起作用，默认换行*/
	
	font-size: 12px;
	/*对多行的文字溢出的处理*/
	overflow: hidden; 
	text-overflow: ellipsis;
	display: -webkit-box;
	-webkit-box-orient: vertical;
	-webkit-line-clamp: 3;
	/*中文不换行*/
	white-space: nowrap;
	overflow: hidden; 
	text-overflow: ellipsis;
}
```

<div class="box1">符合规范新疆消防法规细节分析解决方法金字塔发件人总积分真好听观化听风</div>

### 5.html中引入css的方式

外部样式  < link rel='stylesheet' href="">

引入样式  @import url("demo.css");       @import "demo.css"; 

行内样式  stytle="width:100px;height:100px;"

嵌入样式   <style>.one{width:100px;}<style>



### **在html中插入logo图片

1.<link rel="icon" type="image/png" sizes="16x16" href="/logo-16.png">

`<link rel="icon" href="favicon.ico(img url)" type="image/x-icon">`

<link rel="shortcut icon" href="favicon.ico" type="image/x-icon">

2.嵌入式  通过style标签

### 6.布局

float   position  box-sizing(对border-box进行)盒子的计算方式      display  z-index

### 7.样式

background  background -color  background -image   background -repeat     background -position  background -attachment   

border     border -width border-style  border-color

新增   background -clip  background -origin   background -size   

​           border-image   border-radius :10px  10px/20px横轴/纵轴  ;左上角开始，顺时针

​           box-shadow阴影

​        轮廓线   outline:1px solid red;  不占布局位置    outline-offset：20px; 偏移    可用阴影模拟多层边框


## 十四、盒子模型：四部分

1.内容区域（content):对应的是css中设置的width、height

2.内填充（padding）：用来调整内容和边框的距离

3.边框（border）：

4.外边距(margin):用来调整元素间的距离

**（一）、padding的设置情况**

1.挨个方向设置

2.一行代码设置：

1）、一个值：四个方向  padding: 50px;

2）、 俩个值：上下、左右   padding: 50px 40px;

3）、三个值：上、左右、下  padding: 50px 40px 30px;

4）、四个值：顺时针方向 padding: 50px 40px 30px 20px;

margin和padding 一样

**（二）、border的设置情况**

1.四个方向一起设置 border:10px solid red;

​            border-width:10px;

​           border-style:solid;

​           border-color：red；

2.单个方向设置

brder-top：10px  solid red;

​     brder-top-width:10px;

​     brder-top-style:solid;

​     brder-top-color：red；

**（三）、快速让元素水平居中**

margin: 0 auto; 只对块元素有作用

（四）、元素实际所占大小的计算

宽=width+左右padding+左右border+左右margin

高=hlight+上下padding+上下border+上下margin

#### （五）、margin-top的bug:

> 给子元素设置的margin-top作用在父元素身上

*同时具备5个条件：

1.第一个子元素

2.父元素没有padding

3.子元素没有浮动

4.父元素没有浮动

5.父元素没有border值

解决办法：1）打破其中任意一个条件

​                   2）给父元素设置overflow:hidden

#### （六）、margin设置垂直方向距离会发生合并，只显示最大的值。

#### （七）、padding没有负值，而margin可以。

#### （八）、行内元素的margin值只能设置左右。

（九）、margin: 0 auto; 只对块元素有作用

## 十五、元素分类*

1.块元素（div ul p) display:block;

特点：依次竖排，且能设置大小，独占一行

2.行内块元素(img)display:inline-block;

特点：依次横排，能设置大小

3.行内元素（a span）display：inline；

特点:依次横排，不能设置大小。

## 十六、web的标准布局格式 ：div（块）+css（层叠样式表）布局方式

### （一）、文档流

文档：页面所展示的内容

流：内容要排列的顺序

页面内容默认的排列顺序：从上到下 从左到右，这样的排列规则称为文档流。

### （二）、浮动引发元素脱离文档流，

1.其他元素视它看不见

2.浮动的子元素撑不开父元素。

解决办法：1.父元素能设大小就设置

​                   2.清除浮动产生的影响【在父元素最后的位置添加一个子元素（不能是行内元素），设置clear：both ；】

​                   3.给父元素设置 overflow：hidden；

## 十七、定位属性：层叠顺序及出血

1.相对定位  position:relative;

​     相对定位相对的是自己原来的位置进行移动。

2.绝对定位    position: absolute;

​    绝对定位是对的是**有定位属性**的父元素，如果父元素没有定位属性，会一级级往上走，直到找到根节点html

​	top: 0;

​	bottom: 0;
​	margin: auto;

​	可以实现任意一个元素的居中，水平，垂直，绝对的，得结合 margin: auto;*

3.固定定位   position: fixed;

​	固定定位相对的是当前的窗口进行定位

4.层级关系用z-index：     -1~999；

​	只有当前元素有定位属性时才会起作用

## 十八、颜色透明度的设置

颜色透明：rgba(0,0,0, .6);       hsla()

内容和颜色一起透明：opacity: .6;     0~1S

	background-color: transparent;
	border: transparent;

3.工业颜色模式

H：Hue(色调)。0(或360)表示红色，120表示绿色，240表示蓝色，也可取其他数值来指定颜色。取值为：0 - 360

S：Saturation(饱和度)。取值为：0.0% - 100.0%

L：Lightness(亮度)。取值为：0.0% - 100.0%

## 常用动画

cursor: pointer;   选中后箭头变为手指

box-shadow:0 8px 20px 5px #e0e0e0;  选中后有阴影

transform: translateY(-4px);  选中后纵轴旋转4px

font-weight: normal;  字体不加粗

border:transparent;边框变为透明

##### 过渡 transition

**transition: all 1s linear;  过渡  只在元素上加，任何变化都为1s

* transition: bottom 1s linear;  过渡的属性   时间长短 匀速
  * * transition-property 规定应用过渡的 CSS 属性的名称
  * transition-duration 持续时间（过渡花费的时间
  * transition-timing-function  函数（规定过渡效果的时间曲线
  * ​ transition-delay 延迟（规定过渡效果何时开始

##### @keyframe 规定动画   animation

```
@keyframes rotate {
   		 0%{
			transform: rotate(0deg);
		}
		100%{
			transform: rotate(360deg);
			
		}
}
		animation-name: rotate; 	规定 @keyframes 动画的名称
		animation-duration: 5s;    	规定动画完成一个周期所花费的秒或毫秒
		animation-timing-function: linear;  规定动画的速度曲线
		animation-delay: 2s;     	规定动画何时开始
		animation-iteration-count: infinite;    规定动画被播放的次数：无数次
		animation-direction: alternate;    规定动画是否在下一周期逆向地播放：正反交替
		animation-fill-mode: forwards;
		div:hover{
			animation-play-state: paused; 规定动画是否正在运行或暂停
		}
```

##### 图片左右键

	.dajuhui_huadong{ 图片的左右移动的图标
		width: 35px;
		height: 60px;
		text-align: center;
		line-height: 60px;
		opacity: 0;
		font-size:40px;
		position: absolute;
		top: 0;
		bottom: 0;
		margin: auto;
	}
	.dajuhui_bottom:hover .dajuhui_huadong{ 当选中大图时，左右键出现
		opacity: 1;
		border: 1px solid #DDDDDD;
		background-color: rgba(248, 247, 248, .6);
		color: #DDDDDD;
	}
	.dajuhui_bottom .dajuhui_huadong:hover{ 当选中左右键时，左右键变色
	    color: #343434;
	}
	.dajuhui_lbtn{  左键
	    left: 0;
	}
	.dajuhui_rbtn{  右键
	    margin-right: 200px;
	 	right: 0;
	}
##### 覆盖一层：

宽高同等，颜色接近透明，绝对定位

	.shipin_img2{
		width: 390px;
		height: 227px;
		background-color: rgba(0, 0, 0, .1);
		position: absolute;
		bottom: 0;
		left: 0;
	}
## 十九、渐变

<!DOCTYPE html>
<html lang="en">
<head>

	<meta charset="UTF-8">
	<title>Document</title>
	<style>
		.box{
			width: 200px;
			height: 200px;
			/*background: red  blue;*/
		/*线性渐变*/
	
			/*均匀的渐变*/
		    background: -webkit-linear-gradient(red,yellow,green,cyan,blue,plum);    /*谷歌浏览器和safari*/
		    background: -moz-linear-gradient(red,yellow,yellow,green,cyan,blue,plum);  /*ff*/
		    background: -o-linear-gradient(red,yellow,yellow,green,cyan,blue,plum);   /*opera*/
		    background: linear-gradient(red,yellow,green,cyan,blue,plum);      /*标准语法*/
			/*不均匀的渐变*/
		   ** background: linear-gradient(red 10%,orange,yellow 20%,green 30%,cyan,blue,plum);/*标准语法*/
	
		    background: -webkit-linear-gradient( right,red 10%,orange,yellow 20%,green 30%,cyan,blue,plum);/*标准语法*//*标准语法只写起始位置*/
		    
		/*带方向的渐变(标准语法要加to)*/
		    background: linear-gradient(to left,red 10%,orange,yellow 20%,green 30%,cyan,blue,plum);/*标准语法*/
			/*角度渐变*/
			background: -webkit-linear-gradient( -135deg,red 10%,orange,yellow 20%,green 30%,cyan,blue,plum);/*标准语法*//*标准语法只写起始位置*/
	
			background: linear-gradient(180deg,red 10%,orange,yellow 20%,green 30%,cyan,blue,plum);/*标准语法*/



		/*重复的渐变*/
			**background: repeating-linear-gradient(180deg,red 10%,orange 20%,yellow 20%,green 30%,cyan 20%,blue 20%,plum 20%);/*标准语法*/
		}
		/*0      从下到上
		90     从左向右
		45       左下到右上
		135      左上到右下*/
		.box1{
			width: 400px;
			height: 400px;
			**background: radial-gradient(red 10%,orange 60%,yellow 20%);
		/*正圆*/
			background: radial-gradient(circle,red 10%,orange 60%,yellow 20%);
		/*中心点位置*/
			background: radial-gradient(circle at 10% 30% ,red 10%,orange 60%,yellow 20%);
			background: -webkit-radial-gradient(circle  10% 30% ,red 10%,orange 60%,yellow 20%);
		/*大小的设置（边)*/
			background: radial-gradient(circle closest-side at 10% 30% ,red 10%,orange 60%,yellow 20%);
			background: radial-gradient(circle farthest-side at 10% 30% ,red 10%,orange 60%,yellow 20%);
			     /*(角)*/
			background: radial-gradient(circle closest-corner at 10% 30% ,red 10%,orange 60%,yellow 20%);
			background: radial-gradient(circle farthest-corner at 10% 30% ,red 10%,orange 60%,yellow 20%);
			
			**background: repeating-radial-gradient(180deg,red 10%,orange 20%,yellow 20%,green 30%,cyan 20%,blue 20%,plum 20%);
		}
		.box3{
			width: 300px;
			height: 300px;
			padding: 30px;
			
			border: 20px solid transparent;/*不设置border颜色*/
			background: linear-gradient(white,white) padding-box,url('img/46.jpg') border-box;
			/*先设置文本背景色*/
	
		}    
		.wenzi {
			width: 500px;
			font-size: 60px;
			padding: 28px 0;
			text-align: center;
			background: linear-gradient( to right,yellow, blue,red,green,orange,plum);
			
			-webkit-text-fill-color: transparent;/*文字填充色 透明*/
			
			-webkit-background-clip: text;/*绘制区域从文本*/
			background-position: 0,0;
			background-size: 200% 100%;
			
			animation:piao 4s linear alternate infinite; 
			 				 /*匀速	 往返一次			重复*/
		} 
		/*自定义动画    */
		@keyframes piao{
			0%{
				background-position: 0,0;
			}
			100%{
				background-position: 100%,0;
			}
		}  
	</style>
</head>
<body>
	<!-- <div class="box"></div> -->
	<!-- <div class="box1"></div> -->
	<div class="box3">秋天的枫叶,这是背景边框，</div>
	<h1 class="wenzi">渐变文字</h1>
</body>
</html>

## 二十、背景图

<head>

	<meta charset="UTF-8">
	<title>Document</title>
	<style>
		body{
			background-image: url('img/2.jpg');
			background-repeat: no-repeat;
			background-size: 100% 60%;
			/*设置背景图是否根据内容滚动*/
			background-attachment: fixed;固定
		}
		.box{
			width: 400px;
			height: 1200px;
			padding: 30px;
			border: 50px solid rgba(0, 0, 0, .6);
			/*背景颜色*/
			background-color: red;
			/*背景图片*/
			background-image: url('img/1.jpg');
			/*背景图平铺与否*/
			background-repeat: no-repeat;
			/*背景图大小(长度 百分比 contain cover)*/4种
			/*background-size: 100% 100% ;*/
			background-size: contain;/*包含 图片不变形 图片会完整显示 但会出现覆盖不完整*/
			*background-size: cover;图片覆盖整个盒子，但显示不完整
			/*图片位置*/	
			background-position:  top center;/*center*/
			/*设置图片裁剪区域*/
			background-clip: border-box; 默认             /*padding-box*/
			/*设置图片绘制的位置*/
			background-origin: padding-box;默认
		}
	</style>
</head>
<body>
	<div class="box"></div>
</body>

## 二十一、雪碧图

<!DOCTYPE html>
<html lang="en">
<head>

```
<meta charset="UTF-8">
<title>图片精灵技术/雪碧图</title>
<style>
	.lion{
		width: 52px;
		height: 52px;
		background-image: url('img/index.png');				background-image: url('../img/index.png');
		background-position: -93px -26px;  横（宽）  竖（高）
	}
</style>
```

</head>
<body>

```
<div class="lion"></div>
```

</body>
</html>

## 二十一、阴影及2D转换

### 转换

		transform-origin  perspective   transform-style  perspective-origin
		     translate     x    y  z   3d
		     rotate()  rotateX()  rotateY()  rotateZ()  rotate3d()
		     scale()  x    y    
		     skew()  x y
		     matrix()
<head>

### 阴影

	<meta charset="UTF-8">
	<title>阴影</title>
	<style>
		.box{
			width: 100px;
			height: 100px;
			margin: 20px auto;
			background-color: plum;
		}
		.box:hover{
			box-shadow:0 10px 20px 5px #000;
		/*box-shadow:内外阴影 x y 模糊度 size color;*/
		}
		.qiqiu{
			width: 190px;
			height: 190px;
			background-color: blue;
			margin:0 auto;
			border-radius: 95px 100px 30px 100px;
			box-shadow:inset 20px -3px 20px 5px rgba(148, 166, 173, 1);
			/*2D转换：旋转、平移 斜切 放大缩小*/
			/*transform: rotate(45deg) translate(0, 200px)  skewY(30deg) scale(2,2);*/
			transform: rotate(45deg);
		}
	
	</style>
</head>
<body>
	<div class="box"></div>
	<div class="qiqiu"></div>
</body>

## 二十二、3D（正方体）【2.7

<style>

		*{
			margin: 0;
			padding: 0;
			list-style: none;
		}
		body{
			background-color: #000;
		}
		.box{
			width: 500px;
			height: 500px;
			border: 1px solid red;
			margin: 50px auto;
			/*设置景深以及位置*/
			perspective: 1800px;
			perspective-origin: left top;
			position: relative;
	
		}
		.box ul{
			width: 200px;
			height: 200px;
			/*background-color: yellow;*/
			position: absolute;
			left: 0;
			right: 0;
			top: 0;
			bottom: 0;
			margin: auto;
			-webkit-transform-style: preserve-3d;
			-moz-transform-style: preserve-3d;
			-ms-transform-style: preserve-3d;
			transform-style: preserve-3d;
	
		}
		.box ul li{
			width: 100%;
			height: 100%;
			position: absolute;
			top: 0;
			left: 0;
			transition: all 2s linear;
		}
		
		.box:hover .left{
			background-color: red;
			transform: translateX(-100px) rotateY(90deg);
			 
		}
		.box:hover .right{
			background-color: pink;
			transform: translateX(100px) rotateY(90deg);
		}
		.box:hover .top{
			background-color: blue;
			transform: translateY(-100px) rotateX(90deg);
		}
		.box:hover .bottom{
			background-color: orange;
			transform: translateY(100px) rotateX(90deg);
		}
		.box:hover .before{
			background-color: plum;
			transform: translateZ(-100px);
		}
		.box:hover .after{
			background-color: green;
			transform: translateZ(100px);
		}


	</style>
</head>
<body>
	<div class="box">
		<ul>
			<li class="left"></li>
			<li class="right"></li>
			<li class="top"></li>
			<li class="bottom"></li>
			<li class="before"></li>
			<li class="after"></li>
		</ul>
	</div>
</body>

## 二十三、浏览器内核

**谷歌浏览器：Google Chrome。**  谷歌浏览器之前一直使用苹果的webkit内核，但是现在它与苹果内核分道扬镳，自己开创了新的**blink**内核，这个内核也在被欧鹏（opera浏览器）共同采用和开发；

**火狐浏览器：Mozilla Firefox。**    内核是**Gecko；**

**欧鹏浏览器：OPera。**            内核是blink；

**苹果浏览器：Safari。**      内核:webkit。

IE浏览器：Windows Internet Explorer。   微软出品的浏览器，IE4以上版本都是**Trident**内核。由于垄断性，IE在很长一段时间内没有更新，导致两个后果：一是IE与W3C标准脱节，二是Trident内核大量的bug问题没得到及时解决。所以这就给了其他浏览器机会，比如firefox等。也正是这些原因，使Web前端开发人员大费折，特别是IE6正处在新旧交替的关键地方（已经逐渐被舍弃）.



一些国内的浏览器他们的内核： 
搜狗浏览器：兼容模式（IE：Trident）和高速模式（webkit） 
傲游浏览器：兼容模式（IE：Trident）和高速模式（webkit） 
QQ浏览器：普通模式（IE：Trident）和极速模式（webkit） 
360极速浏览器：基于谷歌（Chromium）和IE内核 
360安全浏览器：IE内核

## 二十四、表单

<!DOCTYPE html>
<html lang="en">
<head>

	<meta charset="UTF-8">
	<title>表单元素</title>
	<style>
		outline：2px solid red;


	</style>
</head>
<body>
	<form action="提交的地址" method=" 提交的方式  get  post">

	表单控件：类型
	            input(text  password  radio  checkbox  file  hadden  submit  reset  button)
	              h5新增[email url date week  month time datetime-local number range滑块展示效果 search color]
	         属性
	            type  name  value  readonly  disable checked maxlength
	            验证required    placeholder
		<label for="">用户名</label>
		<input type="text" value="" placeholder="请输入用户名" maxlength="6" minlength="2">
	
		<br>
	
		<label for="">密码</label>
		<input type="password" value="123456" >
	
		<br>


		<input type="button" value="登录" >
		<input type="submit" value="注册" >
		<input type="reset">
		<br>
	
		<label for="">记住密码</label>
		<input type="radio" name="123" >
	
		<label for="">忘记密码</label>
		<input type="radio" name="123" >
		<br>
	
		<label for="">男</label>
		<input type="radio" name="sex" >
	
		<label for="">女</label>
		<input type="radio" name="sex" >
	
		<br>
	
		<label for="">爱好</label>


		<label for="">爱</label>
		<input type="checkbox">
	
		<label for="">好</label>
		<input type="checkbox">
	
		<br>
	
		<label for="">多行文本</label>
		<textarea name="" id="" cols="30" rows="10"></textarea>
		<!-- style="resize:none;"可实现禁止缩放
		一般情况下textarea 的宽和高是用属性cols 和rows来设置的，如果想要更好的控制的话，就得用CSS来控制，
		textarea{
		    width:600px;//初始宽度
		    max-width:750px;//最大宽度
		    height:60px;//初始高度
		    max-height:100px;//最大高度
		    overflow-y:auto;//让滚动条自适应，保证兼容性
		}

如果禁止所有方向的拉动也可以使用属性resize: none;来控制。
resize属性值：both（表示横向纵向均可拉动）horizontal（表示只有横向可以拉动）vertical（表示只有纵向才可以拉动）none（禁止拉动）
PS：最好不要用百分比来设置textarea宽度~~~~-->
		<br> 

		<input type="tel">
		<input type="email">
		<input type="color">
		<input type="range" max="10" min="-1" value="8">
		<input type="submit" value="注册" >


	</form>
	  action用来指定数据的处理文件
	  method用来指定数据提交方式
	  *get：速度快 不安全
	  *post：速度慢 安全 
	  type：属性用来指定input控件类型
	  value: 设置input的默认值
	  placeholder：用来设置提示信息
</body>
</html>



## 二十六、伪元素（太极）【2.7

1.background-image: linear-gradient(#000   50%,     #fff  50%,                   #fff 100%); 

​                                                                                         开始位置                      结束位置

2.border-top: 200px solid #fff;

   background-color: #000;


## 二十七、移动端

### 1.设计稿

 设计稿：  750*1334  100**100
 iponne8   375*667  50**50
 i7plus       414*736   55.2**55.2

    pc端：1物理像素 =1 逻辑像素
    移动端：1物理像素=多个逻辑像素

单位：rem 倍   （根节点字体大小变化）
1rem    100px
750设备下 font=100px   1rem=100px；
375            50px          50px
414            55.2px        55.2px
em （根据当前元素字体大小）

### 2.弹性布局

css3中新增的布局方式：弹性布局，存在的目的是为了让盒子模型最大程度上灵活性更高，但凡设置了弹性布局，元素身上的float，clear等的属性将消失。

#### 容器（父元素）：

（一）display: flex; 将某个元素变为容器  块元素

​            display:inline-flex;  行内块元素和行内元素

```

（二） 设置项目的排列方式
		flex-direction: row;/*默认*/    横排
		flex-direction: row-reverse;   反向横排
		flex-direction: column;         竖排
		flex-direction: column-reverse; 反向竖排
（三）设置项目的包裹方式
		flex-wrap: nowrap; /*默认*/ 不换行
		flex-wrap: wrap;             换行top-bottom
		flex-wrap: wrap-reverse;     换行bottom-top
(四)项目的水平对齐方式
		justify-content: flex-start;/*左边*/
		justify-content: flex-end;右边
		justify-content: center;     居中
		justify-content: space-between; 俩端
		justify-content: space-around;/*等间距对齐*/
(五)多行项目的垂直对齐方式
		align-content: flex-start;/*项目多行垂直对齐*/
		align-content: center;
		align-content: flex-end;
		align-content: space-between;
		align-content: space-around;
（六）	单行项目的垂直对齐方式	
		align-items: flex-start;默认   上
        align-items: flex-end;     下
        align-items: center;       中间
        align-items: baseline;以文字基线对齐
        align-items: stretch; 延长      只有项目高度不设置或为auto的时候起作用，该项目自动站满整个父元素。
```

#### 项目(子元素):

（一）、项目的排列顺序

order：0; （默认） 数值越小越靠前

（二）、项目的按比例放大

 flex-grow: 0; （默认） 如果某个项目设置为1，会自动计算剩余空间，进行等比例放大。

（三）、项目的按比例缩小

flex-shrink: 1;  （默认） 0或1

如果某个项目设置为0，将不会缩小，如果设置负值，不起作用。

（四）、给项目设置固定宽度

flex-basis: 300px;  默认值是auto，

（五）、设置项目自己的对齐方式

align-self: flex-start;

align-self: flex-end;

align-self: center;

align-self: baseline;  以文字基线对齐

align-self: stretch;   高度延伸

## 3.撑开一屏大小

/* width: 100vw;/* 设备宽度 

	height: 100vh;/* 设备高度 分成100份
	background-color: plum;
	position: fixed;
	left: 0;
	top: 0;
	bottom: 0;
	margin: 0 auto;
	z-index: 999; */


	position: absolute;
	left: 0;
	right: 0;
	top: 0;
	bottom: 0;
	background-color: green;

## 4.隐藏滚动条

hours::-webkit-scrollbar,#day::-webkit-scrollbar{

​                      display: none;        /* 隐藏 */

​                 /* display: block; */

}

## 总结

1.html     hyper text MarkUp language 超文本标记语言

2.标记/标签

【1 行标签 不会独占一行 不能设置宽高   a (href     title     target目标的位置) span   i斜体   em  b  strong      time  address   progress

【2 块标签  独占一行     div   h1~h6  p  pre   ul  li  ol  dl  dt  dd        header    section    main      video  audio   form

【3 行内块级标签   不会独占一行，可以设置宽高    img( src  alt  width height  border)    input  textarea   select  option   fieldset

3.实体  &nbsp    &lt   &gt  &quot  &amp        +;



<th colspan="3">001</th>

<td rowspan="2">003</td>

ctrl alt L   自动整理代码

# 贰、javaScript

### 一、网页有三部分组成：

1.结构层 （html)

2.表现层（css）

3.行为层（javascript）

### 二、定义

javascript  一门语言  计算机语言 编程语言（计算机脚本语言)  一门可以运行在浏览器的脚本语言

### 三、功能

1.完成一些表单的验证

2.制作一些网页效果

3.对于网页的内容进行读写

4.进行一些数据的操作

5.开发网页游戏

6.开发网页应用

7.进行后台开发（Node.js)

### 四、发展历史

1995年 网景公司 布兰奇艾奇 liveScript    javaScript

1995年 微软 IE     Jscript

1996年 javaScript   提交到 ECMA欧洲计算机协会      制定计算机行业的标准

1997年 ECMAScript1.0

1998年 ECMAScript2.0

1999年 ECMAScript3.0

2005年 ECMAScript4.0 没有正式发布

2010年 ECMAScript5.0

2015年 ECMAScript6.0  

2015年

。。。。ECMAScript2017

### 五、组成

ECMAScript   核心语法 （变量 数据类型 流程控制 函数 数组 对象。。。）

BOM Browser Object Model 浏览器对象模型 （如何用js控制浏览器）

DOM Document Object Model 文档对象模型 （如何用js控制文档）

### 六、语法特点

基于对象和事件驱动的解释型松散型语言

### 七、引用方式

1.a链接或者重定向的位置进行调用 

* <a href="javascript:alert(1)">链接</a>

* <form action="javascript:alert(2)">

  ​	<input type="submit" >
  </form>	

2.在事件的后面进行调用    <div onclick="alert(3)"></div>

3.嵌入方式

* <script>

     alert(1);</script>	

4.引入方式      <script src="index.js"></script>

*用于引入的Script标签是不能再插入其它内容的

*采用不同的方式引入的js代码最终还是在一起执行的 所以互相之间还是有联系的

### 八、变量

1.存储数据的容器

2.声明变量 var（关键字）    var 变量名

3.变量赋值

*  声明的同时赋值  var 变量名=值

*  先声明 后赋值     var 变量名;           变量名=值;

*  一次性声明多个变量 然后赋值       var  变量名1,变量名2,变量名3； 变量名1=值；

*  一次性声明多个变量的同时进行赋值   var  变量名1=值,变量名2=值；

*  解构赋值

   ```js
    let arr=[4,6,9,25];
    let [a,b,c,d]=arr;//4 6 9 25
    let [a,b,c]=arr;//4 6 9
    let [m,o,p,l,k]=arr;// 4 6 9 25 undefined
   ```

   剩余运算符  . . . 扩展运算符

   ```javascript
   let arr=[4,6,9,25];
   let [x,y,...z]=arr;//  4 6 [9,25]
   ```

   ```javascript
   let a=1,b=2;
   let [q,w]=[b,a];//2 1
   ```

### 九、ES6 新增的声明方式   let

### 十、ES6 新增的常量声明方式  const 常量名=值

* const PI=3.141596;      只能直接写值，不能先定义后赋值

### 十一、声明覆盖的问题

1.变量值是可以进行重新赋值的 常量不可以

2.var 是可以重新声明的  let和const不可以

3.不使用任何关键字声明  直接给变量赋值是不会报错的

### 十二、变量命名的规范

1.变量命名是严格区分大小写的

2.开始必须是字母或者下划线或者$  

​	  后续可以跟字母 数字 下划线 $

3.不+能使用关键字和保留字

4.js当中的命名习惯   驼峰命名法  	首字母大写

* getElementsByClassName      Date()    Object()

5.变量的命名一定要有实际意义

### 十三、数据类型

1.数值 Number        10    1000000000    1.001    -10000     1e+2   十六进制0x    八进制0o/0    二进制 0b

2.字符串类型 String            " " " "     内容不可换行         ES6 ``模板字符串  内容可换行

* 引号嵌套    单引号和双引号只能互相嵌套     不能自己嵌套自己   但是单引号可以

3.布尔值   Boolean            true和false

4.undefined 	 js特有   只有一个值undefined  一个特殊的值 

* 在某些情况下，变量没有被赋值就会被自动赋值为undefined

5.空值  null    只有一个值null 一个占位符   表示空   一般用于解除对象的引用

6.Symbol 类型    var sl=Symbol();

7.对象  Object   	函数 数组...   	var obj={};

### 十四、数据类型的划分

1.初始类型 	数值	字符串	布尔值	 undefined 	null 	Symbol

2.引用类型 	对象

* 代码在运行的时候数据都是保存在计算机的内存当中
* 内存当中是分为 栈区 堆区
  * * 栈区中保存的都是长度固定的值所占空间比较小	读取速度快
      * * 堆区中保存的是长度可变的值所占空间较大访问速度相对慢些
* js在运行的时候 
* * 初始类型都是在栈区中保存 
  * * 引用类型都是在堆区中保存 只在栈区中保存一个引用地址

### 十五、运算符

1.算术运算符     +	 -	 *	 /	 %  	++	 --

* +还可以用来连接字符串 只要+左右的值只要有一个是字符串，最终结果就是拼接后的字符串
* 如果字符串中全部都是数值（“12345”） 也可以进行除了+之外的算数运算   
* 在算数运算中如果得不到最终的结果 会得到一个NaN (Not a Number)

2.关系运算符（比较运算符）

* 运算结果是布尔值


*  <  >   <=     >=   ==   ===   !=    !==
*  其他类型的比较
*  * 数值和由数值组成的字符串是可以比较的 数值和其他字符串比较结果是flase
  * ==只比较数值大小是否相等  ===不仅要比较数值大小是否相等 还有比较数据类型是否相同
  * 字符串和字符串比较 是从第一位开始  依次比较字母所对应的ASCII码的大小

3.赋值运算符

*  += 	 -=	   *= 	 /=  	%=        eg：num3=num3+5；   等于  num3+=5；

4.逻辑运算符

* 与运算 并且 &&              或运算  或者 ||       非运算  排除 !
* 对于布尔值进行运算 
* * 与运算     同真才为真
  * 或运算     有真则为真
  * 非运算      假值变为真值   真值变为假值
    * * 对于其他类型的值进行运算  假值（0  NaN	 "" 	underfined	 flase 	null)
    * 与运算  值1   值2   结果 
    * ​            真       假        假
    * ​             真1     真2      真2   
    * ​             假1     假2       假1
    * 或运算  值1   值2   结果 
    * ​              真       假        真
    * ​             真1     真2      真1  
    * ​             假1     假2       假2
    * 非运算   假值变为真值   真值变为假值

5.一元运算符

* typeof 判断数据类型	 + 正号	  -负号	   new   	 delete

6.三元运算符(三元表达式)

* 关系运算表达式?当表达式为真的时候的值：当表达式为假的时候的值

* 关系运算表达式可以被替换为任意的一个表达式 

    var a=1;

    var b=a?1:0;

    console.log(b);  得1	

* 表达式     本身就是一个值或者是用来求值的代码

7.特殊运算符

​	( )  1.提升算数优先级  2.调用函数

8、扩展运算符  ...      es6语法



### 十六、流程控制

##### 1.流程

* 代码执行的顺序和方式

##### 2.流程控制

用一些特殊的语句控制程序按照我们想要的方式去选择执行或者是重复执行

##### 3.顺序结构

* * 代码正常的执行顺序 首先按照引入的顺序一块一块执行 在每块当中 从上往下每条语句依次执行
* * 使用var声明变量 在当前代码块中会优先解析

##### 4.选择结构

* 分支结构
* * 单路分支
  * * if(表达式){当表达式为真的时候要执行的代码}
* * 双路分支
  * * if(表达式){当表达式为真的时候要执行的代码}else{当表达式为假的时候的代码}
* * 多路分支
  * if(表达式1){当表达式1为真的时候要执行的代码}else if(表达式2){当表达式2为真的时候要执行的代码}else if(){}...else{}
* * 嵌套分支
  * * 在一个分支结构中嵌套另外一个分支结构

##### 5.条件结构（2.27>index.html)

switch(表达式){

​	case 值1：当表达式的值为1时要执行的代码;

​	break;

​	case 值2：当表达式的值为2时要执行的代码;

​	break;

​	.....

​	default:当表达式的值和所有值都不匹配的时候要执行的代码

}

##### 6.循环结构

* for循环


   for(var i=0;i<20;i++){
   		console.log(1);
   	}
   	var sum=0;
   	for(let i=1;i<=100;i++){
   		sum+=i;
   	}
   	console.log(sum);
* while循环

  while(表达式){

  ​	当表达式的值为真时要执行的代码;

  }

  ​

  ```javascript
  	 var grade=prompt("请输入成绩");
  	while(!(grade>=0&&grade<=100)){
  	 	grade=prompt("请输入成绩");

  	}
  ```

* do while循环

* do{

  ​

  }while{

  ​

  }

  ​

  ```javascript
  	var grade;
  	do{
  		var grade=prompt("请输入成绩");
  	}while(!(grade>=0&&grade<=100))
  ```

成绩判断 计算器的的实现 累加运算 求闰年  求偶数 十行十列表格 99  金字塔 鸡兔同笼    2遍

##### 7.控制语句：

break终止循环	 continue停止当前循环，执行下一次循环

### 十七、函数

> 函数就是封装起来可以被重复调用的代码块

##### 2.好处

* 使程序更加简洁
* 维护更加方便
* 逻辑更加清晰

##### 3.函数的声明

* 使用function关键字	函数名的命名规则和变量名是一样的 	函数名不能和变量名重复  会被优先解析【后面script中或引入都可以】

  function		函数名(参数 ){

  ​	//函数（主）体

  }

  ```javascript
  	//说明优先性
  	a();
  	function a(){
  		alert(2);
  	}
  ```

* 匿名函数

  * var fn=function(){}

      		var foo=function(){
      			alert(3);
      		}
      		foo();

  * setInterval(function(){},1000);

  * div.onlick=function(){}

* 实例化构造函数

  * var fn=new Function();

      			var bar=new Function("alert(33)");
      			bar();

##### 4.函数的调用

函数名（）  变量名（）

1）在事件的后面调用

<script>

```javascript
var ele=document.querySelector(".demo");
ele.onclick=function(){
	alert(2);
}
```

</script>

2）自调用（自己调用自己)

```javascript
(function(){	
	alert("函数自调用");
})();
```
##### 5.函数的参数

让函数的调用更加灵活

* 参数 分为实参和形参
  * 实参  调用函数的时候传递的真正的值
  * 形参  在声明函数的时候定义的变量
* 参数的个数可以是多个
* 参数的数据类型  任意的数据类型
* 参数的默认值
* 实参的个数超出形参的个数
* 每声明一个函数 函数的内部都会自动生成一个arguments对象  arguments对象会保存所有传递的实参

##### 6.函数的返回值

> 函数的返回值是定义在函数内部的语法结构 返回的值就是函数调用表达式的结果

* return 返回值;
* return 返回值只能有一个
* return 语句之后的代码会被自动忽略
* 可有可无 可以返回任意需要的值

##### 7.函数的重载

> 根据参数的个数和类型的不同执行不同的函数体

##### 8.环境

* js代码的执行分为两种环境执行
  * 全局环境
  * 函数环境
* 任何一条语句在执行前要先解析当前所处的环境
* 如果在全局环境中声明一个变量  在整个全局环境中都可以访问到这个变量  也就称作当前的变量拥有全局的作用域 这个变量被称作全局变量
* 如果是在函数环境当中声明一个变量 在这个当前的函数环境中都可以访问到这个变量 也就当前的变量的作用域只在函数当中 被称作局部变量
* 实际的原因 在某一个函数运行结束之后 函数内部声明的变量都被销毁掉了
* 1.保证全局变量不受污染   2.方便进行变量命名
* 函数的作用域和变量的作用域拥有完全相同的表现特征

##### 9.作用域链

> 当我们访问某个变量的时候，会先从当前变量所在环境中进行解析，如果在当前环境中找不到，则到当前环境的外部环境中寻找，一直找到全局环境为止。

10.块级作用域（let和const声明的变量只能在这个作用域内，外部不能调用

if(){} 	for(){}	while(){}	do{}while()  {}	

##### 11.递归函数

> 在函数的内部自己调用自己 一般有设置不在递归调用的出口

* 参数一定是发生改变的

##### 12.回调函数

> 把一个函数做为另一个函数的参数使用   这个函数就被称为回调函数

##### 13.闭包**

> 让函数当中定义的局部变量在函数运行结束之后不被销毁的一种手段
>
> 实现方式：在函数的内部定义另外一个函数并将他返回 在这个函数中可以访问函数内部定义的变量

##### 14.内置顶层函数

> 在js内部定义好的拥有全局作用域的一些函数

* eval();  对参数引号内部的内容按照js的语法进行解析    eval("alert(1)");

* Number();   将其他的数据类型转化为数值类型 

    //Number
    ```javascript
    j	console.log(Number("123"));  //123
    	console.log(Number("abc"));  //NaN
    	console.log(Number("123abc"))  //NaN
    	console.log(Number("abc123"))  //NaN
    	console.log(Number(""))  //0
    	console.log(Number("-1"))  //-1
    	console.log(Number("0x11"))  //17 十六进制
    	console.log(Number("00011.00"))  //11
    	console.log(Number(true));	//1
    	console.log(Number(false));//0
    	console.log(Number(undefined));  //NaN		
    	console.log(Number(null));	//0
    	console.log(Number({name:"查娜"}));  //NaN
    ```

* parseInt();  将字符串类型转化为数值型

    //parseInt
    ```javascript
    	console.log(parseInt("25852"));  //123
    	console.log(parseInt("abc"));  //NaN
    	console.log(parseInt("123abc"))  //123    左到右
    	console.log(parseInt("abc123"))  //NaN
    	console.log(parseInt(""))  //NaN
    	console.log(parseInt("-1"))  //-1
    	console.log(parseInt("0x11"))  //17 十六进制
    	console.log(parseInt("00011.00"))  //11
    	console.log(parseInt(true));	//NaN
    	console.log(parseInt(false));//NaN
    	console.log(parseInt(undefined));  //NaN		
    	console.log(parseInt(null));	//NaN
    	console.log(parseInt({name:"查娜"}));  //NaN
    ```
      //第二个参数

    ```javascript
    		console.log(parseInt("11",5))  //表示以几进制的方式解析  5进制
    ```

* parseFloat();  字符串数据类型转化为数值类型

    console.log(parseFloat("123"))  //123
    ```javascript
    	console.log(parseFloat("123.123"))  //123.123
    ```

* String();     将其他的数据类型装换为字符串

    //String();
    ```javascript
    	console.log(String(123));
    	console.log(String(true));
    	console.log(String(false));
    	console.log(String(undefined));
    	console.log(String(null));
    ```

* Boolean(); 将其他数据类型转化为布尔型

* isNaN(); 判断当前的值 进行Number转化后 是不是NaN

##### 15.数据类型转换

* 强制数据类型转换 

* 隐式的数据类型转换

  “5”-“2”     3  在-两边 如果不是数值，自动调用 Number()函数进行转换

  “hello”+2      在+两边 如果一个是字符串 另一个不是 对于不是字符串类型的 自动调用 String()函数进行转换

  10>"5"    在>两边 如果一边是数值 另一边不是 对于不是 对于不是数值的类型 自动调用Number()函数进行转换

  表达式？表达式：表达式  三元表达式的第一个表达式如果不是布尔值 会自动调用 Boolean() 转化为布尔值

  if(表达式){}	表达式如果不是布尔值 会自动调用 Boolean() 转化为布尔值

### 十八、数组

存储一组或一系列相关数据的容器	一种数据类型

##### 1.创建数组

var arr=[ ];

* var arr=[1,2,2,2];
* var arr=[ ];        arr[0]=1; arr[2]=2;...

通过下标可以访问数组中的某个成员，也可以直接给数组设置值

length 属性代表数组的长度 一般情况下指的是数组当中成员的个数，是最后一个有值的下标+1

访问任意一个没有赋值的下标 得到的值是undefined	*4种*

实例化构造函数 new Arrary();  如果只传一个参数 这个参数表示数组的长度

##### 2.二维数组

var arr2=[[98,87,87,54,],[65,63,32,54]];//二维数组

##### 3.根据类型选出数组【3.6】

```javascript
	var arr3=[98,65,32,[98,65,32],[25,45,14,12]];
	for(var i=0;i<arr3.length;i++){
		// console.log(arr2[i]);
		if(typeof arr3[i]==="object"){
			for(var j=0;j<arr3[i].length;j++){
				// console.log(arr3[i][j]);
			}
		}else{
			// console.log(arr3[i]);
		}
	}
```
### 十九、js对象

> 是属性的无序集合体

##### 1.对象(object)

> 任何的客观事物	以及抽象的规则、计划和事件等。

一切皆对象

##### 2.属性

*属性：描述对象当前状态的一些信息（数值 字符串 布尔值 。。。）

*方法：描述对象的行为、动作、功能（函数）

##### 3.类

具有相同或相似属性的对象的抽象描述叫做类

类的具体化或者实例化就是对象

在js中是通过构造函数(function Arrary)来实现类的

new Function()	new Arrary()

##### 4.语法

* 创建一个对象

1）json方式

var obj={name1:"value1",name2:"value2"}

2)先写一个构造函数 再去实例化

function Human(){};

var obj=new Human();//实例化

3)直接实例化顶层构造函数 Object()

var obj=new object();

* 对象属性的添加

  可以在任意的时刻进行添加

* 对象属性的访问

  对象.属性

  对象[变量]

  对象.方法()

  对象[变量]\(\);

* 对象属性的遍历

   ```javascript
   for (var i in person1){
   	console.log(i);
   	console.log(person1[i]);
   }
   ```
* 对象属性的删除

  delete 对象.属性

  delete person1.name;

##### 5.js对象的分类

* 原生对象

在js内定义的语法内部自带的一些对象/构造函数

Array()  String()	boolean()	Function()	Object()	Error()	Date()	RegExp()		Math(数学对象)	JSON   

得到一个原生对象  	new 构造函数()	

* 宿主对象

  1)BOM 浏览器对象模型 window    history	 location 	screen	 document	 navigator

  window 

  属性

  screenleft    screenTop  火狐不能识别

  screenX    screenY    

  innerWidth  

  innerHeight

  localStorage

  sessionStorage

  top   访问父窗口的window对象

  方法：

  alert()    prompt() 弹出输入框 请输入

    confirm()确定    setInterval     clearInterval ()     

  getComputedStyle()获取任意元素的css属性

  setTimeout(function(  ){ },3000)        clearTimeout

  let st=setTimeout(function(  ){ },3000)  ;

   clearTimeout(st);

  2)DOM 文档对象模型 document div a p  span  a... 每一个标签

  获取这些对象有特定的方式

#### 6.document object model 文档对象模型

提供了用js操作页面当中标签 属性 样式 内容的能力

##### 1.操作页面

document对象

   	querySelector()

​	querySelectAll()	

获取元素对象/标签对象 的方法

​	document.querySelector()

​	document.querySelectAll()	

##### 2.元素对象的属性

innerHTML 获取或者设置 标签的内容

className	获取或设置  标签的类名

id	获取或设置 标签的id

style	获取标签的行内样式集合

​	div.style.width 获取或设置某一行内样式

​       div.style.height

classList 获取标签的类名集合对象

​	add()添加某个类名

​	remove()移除某个类名

//tagName 标签名  nodeName

##### 3.元素对象的事件

> 事件：用户对于浏览器的操作 浏览器自身行为

onclick 鼠标单击事件

onmouseenter 鼠标进入事件

onmouseleave 鼠标离开事件

transitionend  过渡结束事件

onsrcoll  元素或者浏览器窗口发生滚动的时候触发的事件  window.onsrcoll

ondblclick  鼠标双击事件    单击在双击后，双击时会有两次单击事件，一次双击事件

onmousedown  鼠标按下事件

onmouseup  鼠标抬起事件

onmousemove  鼠标移动事件

onmouseover  鼠标进入事件 

onmouseout  鼠标离开事件

onmousewheel  google    DOMMouseScrool   火狐

onwheel  滚轮事件



onchange  当选择select 其他选项 

​	 input.onchange=function(){

​		cnsole.log("改变事件");

​	}

onfocus 获得焦点事件   input.onfocus

onblur  失去焦点事件   input.onblur



键盘事件  window document body  可以输入的元素

window.onkeydown  键盘按下事件

window.onkeypress  键盘按压事件

window.onkeyup  键盘抬起事件



动画结束事件

​	floatingwindow.addEventListener("animationtend",function(){

​		console.log("动画效果结束事件")

​	})

文档内容加载完成事件

```javascript
<script>
	window.onload=function(){
		var items=document.querySelectorAll(".item");
		console.log(items);
	}
</script>
```
##### 4.元素对象的方法

addEventListener (事件类型,事件处理程序（程序）)        添加事件监听   可以给一个事件添加多个监听

```javascript
floatingwindow.addEventListener("transitionend",function(){
	this.onclick=function(){
		this.style.display="none";
	}
})
```
单线程

```javascript
floatingwindow.addEventListener("click",function(){
	console.log(1);
})    //点击事件  和用onclick一样
floatingwindow.addEventListener("click",function(){
	console.log(2);
})
```
removeEventListener 移除监听

```javascript
function handler(){
	console.log(1);
	console.log(1);
	console.log(1);
	console.log(1);
	console.log(1);
}
div[0].addEventListener("click",handler);
div[0].addEventListener("click",function(){
	console.log(2);
	console.log(2);
	console.log(2);
	console.log(2);
})
div[0].removeEventListener ("click",handler);
```
querySelector()

querySelectAll()

documentElement.scollTop

##### 5.事件对象

保存事件触发的时候产生的一系列信息

let demo=document.querySelector(".demo");

```javascript
demo.onclick=function(e){
	//属性
	console.log(e.screenX);  //相对于电脑屏幕
	console.log(e.screenY);
	console.log(e.clientX);  //相对于当前浏览器窗口位置
	console.log(e.clientY);
	console.log(e.pageX);  //相对于当前文档左上角位置
	console.log(e.pageY);
	console.log(e.offsetX);  //相对于当前事件源
	console.log(e.offsetY);

	console.log(e.type); //当前事件的名称
}
demo.addEventListener("click",function(e){
	console.log(e);
});
window.onkeydown=function(e){
	console.log(e.keyCode);
	console.log(e.ctrlKey);  //判断键盘码是否是按下状态
	// console.log(e.shiftKey);
	// console.log(e.altKey);
}
```
### 二十、继承&原型   mdn进行查找【3.7】

##### 1.继承

> 在一个类中通过某种方式获得另一类当中所有的属性和方法，这种方式叫做继承

存在继承关系的类 当我们访问某个类实例化对象的属性的时候会先从当前对象身上找，如果找不到，就会去找类，如果当前类没有，就回去找当前类的父类

##### 2.原型【3.6】

将某个对象的构造函数（类）的prototype属性设置为另一个构造函数（父类）实例化的对象，这个对象就称作某个对象的原型，这种方式就是js实现继承的一种方式

```javascript
	var person1={name:"zhangsan",sex:"man",	
		age:18,
		say:function(){
			alert("hello word");
		}
	};
	// console.log(person1.name);
	// person1.say();

	//json格式
	var cup={
		color:"yellow",
		size:"m",
		owner:"wtt",
		drink:function(){
			console.log("喝水");
		},
		getWater:function(){
			console.log("接水");
		}
	}

	var computer={
		color:"black",
		sixe:"15.6寸",
		owner:"wtt",
		start:function(){
			console.log("开机");
		},
		end:function(){
			console.log("关机");
		}
	}
	console.log(computer.color);
	computer.start();

	function Human(_sex,_age,_name){
		//指的就是将要实例化的对象
		this.sex=_sex;
		this.age=_age;
		this.name=_name;
		this.say=function(){
			alert("hello word");
		}
	}
	var person1=new Human("man",18,"wtt"); //实例化  类...  对象
	console.log(person1);

	var attr=prompt("请输入姓名");
	console.log(person1[attr]);

	for (var i in person1){
		console.log(i);
		console.log(person1[i]);
	}

	delete person1.name;
	delete person1.say;
```
##### 3._ proto _

每一个对象自带的一个访问器属性，这个属性对象身上本身是没有的，是浏览器实现的一个功能，通过_ proto _ 可以访问当前对象的原型

//es5	ie8+

```javascript
j//foreach
	var arr=[1,2,3,4];
	var newarr=[];
	// arr.foreach(function(val,index){
	// 	if(val<3){
	// 		newarr.push(val);
	// 	}
	// })
	// Array.prototype.myForEach=function(callback){
	// 	for(var i=0;i<this.length;i++){
	// 		callback(this[i],i);
	// 	}
	// }
	// arr.myForEach(function(val,index){
	// 	concole.log(val);

	// })
//filter  过滤
	Array.prototype.filter=function(callback){
		var newarr=[];
		for(var i=0;i<this.length;i++){
			var r=callback(this[i],i);
			if(r){
				newarr.push(this[i]);
			}
		}
		return newarr;
	};
	var newarr=arr.filter(function(val){
		if(val<3){
	 		return true;
	 	}

	})
	// console.log(newarr);
//map 映射
	Array.prototype.map=function(callback){
		var newarr=[];
		for(var i=0;i<this.length;i++){
			// var r=callback(this[i],i);
			// if(r){
				// newarr.push(this[i]*this[i]);
				newarr.push(callback(this[i],i));
			// }
		}
		return newarr;
	};
	var newarr=arr.map(function(val){			
	 		return val*val;
	})
	console.log(newarr);

//判断 some every
	var hasfail=arr.some(function(val,index){
		if(val<3){
	 		return true;
	 	}

	})
	console.log(hasfail);

	var allsuccess=arr.every(function(val,index){
		if(val>=3){
	 		return true;
	 	}

	})
	console.log(allsuccess);

//indexOf lastIndexOf 第一次 最后一次出现的位置
	console.log(arr.indexOf(2));
	console.log(arr.lastIndexOf(2));
	console.log(arr.indexOf(10)); //不存在的数结果为-1

//reverse 颠倒数组里每个成员的排列顺序
	arr.reverse();
	console.log(arr);

//reduce 	左到右   reduceRight  右到左
	//val1 上次运算的结果
	//val2 正在遍历的数
	var sum=arr.reduce(function(val1,val2){	
			console.log(val1,val2);		
	 		return val1*val2;
	})
	console.log(sum);
```
//es6

```javascript
//fill
	var arr=new Arrary(10);
	arr.fill(0);
	console.log(arr);
//find
	var grade=[{name:"zhangsan",grade:98},{name:"lisi",grade:78},{name:"wangwu",grade:56}];
	var obj=arr.find(function(val,index){
		if(val.grade=78){
	 		return true;
	 	}
	})
	console.log(obj);
	//findIndex
	//copyWithin
	//includes
```
"use atrict";//触发严格模式	【3.8】

```javascript
	var obj={name:"lii"};
	function fn(val1,val2){
		console.log(this);
	}
	fn.call(obj,1,2);
	fn.apply(obj,[1, 2]);

	// function Human(){
	// 	this.arms=2;
	// 	this.legs=2;
	// }

	// var someone=new Human();

//new
	// var obj={};
	// obj._proto_=Human.prototype;
	// Human.call(obj);
	// someone=obj;

//重点	
	var name="lisi";
	var obj={
		name:"zhangsan",
		o:{
			name:"wangwu",
			fn:function(){
				console.log(this.name);
			}
		}
	}
	obj.o.fn();//wangwu

	var fn=obj.o.fn;
	window.fn(); //lisi

	obj.fn=obj.o.fn;
	obj.fn();  //zhangsan
	// function Human(){
	// 	this.arms=2;
	// 	this.legs=2;
	// 	// console.log(this);
	// }
	// Human.prototype={
	// 	sleep:function(){
	// 		console.log("睡觉");
	// 	}

	// }
	// var someone=new Human();
	// console.log(someone);
```


```javascript
//ES6
	class Human{
		constructor(){
			//Human类的构造函数
			this.arms=2;
			this.legs=2;
		}
		say(){
			console.log("说话");
		}
	}
	class Student extends Human{
		constructor(id){
			super();//执行父类的构造函数
			this.id=46;
		}
		walk(){
			console.log("走路");
		}

	}
	var student=new Student();
	console.log(student);
	var human=new Human();
	console.log(human);
```
##### 4.this

> 在调用函数的时候通过call或apply传递的参数

调用当前方法的对象 

调用事件的时候  this指的是添加事件的对象

call apply  传递的参数

如果在构造函数中 this指的就是实例化的对象

```javascript
imgs.forEach(function(){
	console.log(this)
},{name:"zhangsan"})
```
【3.9】

```javascript
<style>
	div{
		width: 100px;
		height: 100px;
		background-color: red;
	}
</style>
</head>
<body>
	<div></div>
</body>
<script>
//ES5
var div=document.querySelector("div");
var obj={name:"zhangsanlllllll"};
div.onclick=function(){
	console.log(this);
}.bind(obj);//用bind调用
setInterval(function(){	
	console.log(this);
}.bind(obj),3000)
	//只有匿名函数可以绑定this
</script>
```
##### 5.Arrary.isArrary【3.7】-2

```javascript
Arrary.isArrary
	var arr=[56,45,12,[1,2,3],true,null];
	from()
	of()
ES3 ie6 ie7 ie8
	push()  从末尾位置添加
	pop()	删除最后一个数
	unshift()  从开始位置添加
	shift() 删除开始第一个
	splice(位置，删除个数，要添加的个数) 返回值是删除的数组成的数组
				1,	0, 	1
	var arr=[1,2,3,4];
	console.log(arr.push(6,7,8,9));  //返回值是个数 执行的是从末尾位置添加
	console.log(arr); 	
	console.log(arr.pop()); //返回值是删除的最后一个数   执行的是删除最后一个数
	console.log(arr);
	console.log("返回值："+arr.unshift(18,20)); //返回值是个数 执行的是从开始位置添加
	console.log(arr);
	console.log(arr.shift()); //返回值是删除的第一个数 执行的是删除第一个数
	console.log(arr);
	console.log(arr.splice(1,2)); //返回值是删除的数组成的数组  执行的是在任意位置增加或删除
	console.log(arr);
	console.log(arr.splice(1,0,1,0,1,0)); //返回值是删除的最后一个数
	console.log(arr);

	//join
	console.log(arr.join(""));//数组转化为字符串
	console.log(arr);
	//slice
	console.log(arr.slice(3));//从第三个位置起截取到最后位置
	console.log(arr);
	console.log(arr.slice(3,7));//从第三个位置起截取到第七个位置
	console.log(arr);
	console.log(arr.slice(1,-1));//从第一个位置起截取到-1位置
	console.log(arr);
	//concat
	var newarr=["a","b"]; 
	console.log(arr.concat(newarr));//从最后往左拼接
	console.log(arr);
	console.log(newarr);
	//sort
	console.log(arr.sort());//排序
	console.log(arr);
	console.log(arr.sort(function(a,b){
		if(a>b){
			return 1;
		}else{
			return -1;
		}
	}));

	var grade=[{name:"zhangsan",grade:98},{name:"lisi",grade:78},{name:"wangwu",grade:56}];
	grade.sort(function(a,b){
		if(a.grade>b.grade){
			return 1;
		}else{
			return -1;
		}
	});
	console.table(grade);
```
##### 6.ES6中用class定义类

```javascript
	class Human{
		constructor(){
			//Human类的构造函数
			this.arms=2;
			this.legs=2;
		}
		say(){
			console.log("说话");
		}
	}
	class Student extends Human{
		constructor(id){
			super();//执行父类的构造函数
			this.id=46;
		}
		walk(){
			console.log("走路");
		}

	}
	var student=new Student();
	console.log(student);
	var human=new Human();
	console.log(human);
```
##### 7.string

//字符串对象

```javascript
	//
	var str="hello world";
	//属性
	console.log(str.length);
	console.log(str[0]);//ie8+
	console.log(str.constructor);
//方法
	//获取
	console.log(str.charAt(0));//h
	console.log(str.charCodeAt(0));//当前获取的字符的unicode编码
	console.log(str.indexOf("o"));		//4
	console.log(str.lastIndexOf("o"));	//7
	console.log(str.indexOf("c"));		//-1
	console.log(str.indexOf("world"));//6
	console.log(str.indexOf("worlld"));//-1
	//替换
	console.log(str.replace("world","web"));//只能替换一个
	//转换
	console.log(str.split(""));//转换成数组
	console.log(str.split("",10));     //   10 最大长度
	var str="hello";
	str=str.split("").reverse().join("");
	var str="hello world";
	//分割
	console.log(str.slice(1,-1));  //ello worl
	console.log(str.substring(1, 3)); //el          不能接收负数
	console.log(str.substr(4,2)); //o   从4位置截取个2个
	//大小写转换
	console.log(str.toUpperCase());//大写
	console.log(str.toLowerCase());//小写
	//ES5 trim() 去除字符串两端的空格
	var str="  hello world  ";
	console.log(str.trim());
	//ES6 includes() 判断字符串中是否存在某个字符
	console.log(str.includes("o"));  //true
```


```javascript
//String 函数的方法
	console.log(String.fromCharCode(97,98,99));  //根据unicode编码 选出字符
	console.log(str);

	var str1="hello a hello b hello c hello d";
	while(str1.includes("hello")){
		str1=str1.replace("hello","hi");
	}
	console.log(str1);

	var str2="background-color color z-index text-align";
	while(str2.includes("-")){
		var pos=str2.indexOf("-");
		var charcter=str2.charAt(pos+1);
		var UpperCase=charcter.toUpperCase();
		str2=str2.replace("-"+charcter,UpperCase);
	}
	console.log(str2);
```
##### 8. function【3.9】

//ES6 function

```javascript
//1 函数的默认参数
	function table(rows=10,cols=10,color="red"){
		console.log(rows,cols,color);
	}
	table(3,3,"blue");
	table(1);
	table();
//2 箭头函数 
	var arr=[1,2,3,4];
	// var newarr=arr.map(function(){
	// 	return v*v;
	// })
	var newarr=arr.map(v=>v*v);
	
	// var newarr2=arr.filter(function(v){
	// 	// if(v>3){
	// 	// 	return true;
	// 	return v<3;
	// });
	var newarr2=arr.filter(v=>v<3);

	var sum=(a,b)=>a+b;
	console.log(sum(1,6));

	var getPI=()=>3.1415926;

	var fn=n=>{
		alert(n);
		return n;
	}

	// var fn2=function(w,h){
	// 	return {width:w,height:h};
	// }
	var fn2=(w,h)=>({width:w,height:h});

	// div.onclick=()=>{};  事件可以用，但一般不用
//1 箭头函数中没有arguments
//2 箭头函数不会影响当前this的指向
		var name="zhangsan";
		var obj={
			name:"lisi",
			fn:function(){
				console.log(this.name);
				//setInterval(function(){
				setInterval(()=>{	
					console.log(this);
					console.log(this.name);
				},3000)
			}

		}
		obj.fn();
```
##### 9.Arrary String math 数学对象【3.9】

//Arrary String math 数学对象

```javascript
	console.log(Math.abs(-100)); //100  取绝对值
	console.log(Math.abs(100));  //100

	console.log(Math.round(4.4)); //4  四舍五入
	console.log(Math.round(4.5)); //4
	console.log(Math.round(4.9999999));  //5

	console.log(Math.floor(4.99999));  //4  向下取整
	console.log(Math.ceil(4.00001));  //5   向上取整
	console.log(Math.floor(-1.333));  //-2

	console.log(Math.max(1,211,3,254,5));  //254  选出最大值
	console.log(Math.min(-1,211,3,254,5));  //-1

	console.log(Math.random());   //0~1间随机小数
	var arr=["a","b","c"];
	setInterval(function(){
		// console.log(arr.Math.random()*3);
	},3000)

	console.log(Math.random()*50+50); //50~100
	console.log(Math.random()*10+20); //20~30
	console.log(Math.random()*20-10); //-10~10
	console.log(Math.random()*50+50);
	console.log(Math.random()*50+50);
						   *差值+开始值

	var num=Math.random()*26+65;  //A~Z 65~90
	// consle.log(String.fromCharCode(num));
	
	console.log(Math.sqrt(2));
	console.log(Math.pow(2,10));//ES6运算符  2的10次方
	console.log(2**10);
	console.log(Math.sin(Math.PI/6));//角度转为弧度
	console.log(Math.cos());
	//deg rad
	//360deg  2PI
	//180deg  PI
	//1       PI/180
	console.log(Math.PI);
```
##### 10.【3.10】

console.log(getComputedStyle(wtt).width);  当前元素在页面中实际所占的宽度和高度


```javascript
console.log(wtt.offsetWidth);
console.log(wtt.offsetHeight);
//offsetLeft  offsetTop  
//所有的前辈元素都没有定位属性 相对于文档的位置
//如果前辈元素有定位属性  相对于离当前元素最近的有定位属性的前辈元素的位置
console.log(wtt.offsetLeft);
console.log(wtt.offsetTop);
```
scrollTop scrollLeft

```javascript
let totop=document.querySelector(".totop");
totop.onclick=function(){
	document.documentElement.scollTop=0;
}
```
##### 11.Date

```javascript
let date=new Date();//当前的系统时间
console.dir(date);
let future=new Date(2018,2,20,12,0,0);//0~11   年 月日 时间
console.dir(future);     //Tue Mar 20 2018 12:00:00 GMT+0800 (中国标准时间)

//获取当前时间
console.log(date.getYear());//118    1900 1 1 开始到现在的年数
console.log(date.getFullYear());//2018 
console.log(date.getMonth());//2     一月到12月： 0~11
console.log(date.getDate());//20
console.log(date.getDay());//        周一到周六：1~6 周日: 0
console.log(date.getHours());//10    24小时制 0~23
console.log(date.getMinutes());//39
console.log(date.getSeconds());//40  0~59 秒
console.log(date.getMilliseconds());//0-999  毫秒
console.log(date.getTime());//毫秒数   1970 1 1 开始到现在的毫秒数
console.log(date.getUTCDate());
console.log(date.getUTCHours());//国际标准时间 2 现在东八区 快8小时

//设置时间
let newdate=new Date();
newdate.setFullYear(2020);
newdate.setMonth(0);//1月
newdate.setDate(1);//
                    //星期不能设置，是随着日期而定的
newdate.setHours(0);
newdate.setMinutes(0);
newdate.setSeconds(0);
newdate.setMilliseconds(0);
console.log(newdate);  //Wed Jan 01 2020 00:00:00 GMT+0800 (中国标准时间)
```

#### 12、正则表达式

> 描述一段特殊语法规则的表达式

##### 1.用途

用于字符串的替换 检索和拆分等操作

##### 2.场合

各种编程语言

编辑器

浏览器

##### 3.正则对象

1）实例化 new RegExp("uek","g")

2）直接写   /正则的语法 /g

方法：test() 判断字符串是否配当匹前正则

​	  exec()  以当前正则指定的规则对于一个字符串进行解析提取

##### 4.语法

描述普通的字符串

- 定界符 （描述一些边界的符号）

^  描述整个字符串开始的位置

$  描述整个字符串的结束位置

\b  单词的边界

\B 单词中除了边界以外的其它部分



- 原子 (正则当中最小的单位)

\d数字  0~9的任意一个数字  [0-9]

\D  除了0-9以外的其它字符	[\^0-9]

 \s    一个空格

\S   除了空格以外的其它字符

\w  数字 字母 下划线  [0-9a-zA-Z_]

\W  除了数字 字母 下划线以外的其他字符  [\^0-9a-zA-Z_]

\n 换行符

\r  回车键



- 原子表（提供可选的一组数来表示一个原子）

[1-9 ]

[a-z]

[1-9a-z]   

[^1-9]  除了1-9以外的其他字符



- 模式修正符（定义当前正则的匹配模式）

  g (global  全局)    在进行exec()  每一次匹配会从上一次匹配到的位置开始

  ​str.replace();会在替换之后继续查找其它符合条件的 如果有继续替换

i    不区分大小写

m    不识别换行



- 量词（指定当前的原子、原子表或者原子组的个数）

\*       0个或者多个   {0,}      

\+    1个或者多个   {1,}

？  0个或者1个  {0,1}

{3}   三个

{3,5}  三到五个

{10，} 十个以上



- 元字符（在正则当中起特殊作用的符号）

\   转义字符   普通到特殊   特殊到普通

 |   表示或者   

.     匹配任意的字符    不包括换行



- 量词的贪婪与吝啬

本身是贪婪的

如果希望是吝啬 可以在量词的后面加一个？

- 反向引用		每一个用小括号括起来的部分都可以在后面直接引用
  - 取消反向引用     如果不希望某个括号中的内容被引用  在括号的 （？：


- 不获取 正向肯定预读      只匹配  不获取（？=

uek   uek1  uek2 uek3                      

- 不获取 正向否定预读      只匹配  不获取（？！

##### 5.字符串中可以使用正则的方法

replace    替换

search     第一次出现的位置

match     相当于 exec     以当前正则指定的规则对于一个字符串进行解析提取

split    字符串转换为数组

// 补充   细化     讲程序

### 二十一、文档树  文档树模型

定义了节点 和节点的属性方法  console.log(document);

##### 1.节点 HTML DOM：

每一个标签都是一个元素节点    	每一个文本都是一个文本节点	

标签的每一个属性都是一个属性节点		每一个注释都是一个注释节点 	整个文档 称为文档节点

##### 2.节点也是对象

##### 属性

节点的关系属性  commment注释

```javascript
<body>
  <div class="box">
      <div class="item">1</div>
      <div class="item">2</div>
      <div class="item">3</div>
  </div>
</body>
```
<script>
```javascript
let item1=document.querySelector(".item:first-child");
let box=item1.parentNode;  父节点 //<div class="box"> ...</div>	
let childs=box.childNodes;   子节点//7个子元素
let firstChild=box.firstChild;  //#text
let lastChild=box.lastChild;	//#text

let firstElement=box.firstElementChild;//第一个元素节点  <div class="item"> 1</div>
let lastElement=box.lastElementChild;	//<div class="item"> 3</div>

let nextSibling=item1.nextSibling; 下一个兄弟元素//#text
let previousSibling=lastElement.previousSibling;  //#text

let nextElement=item1.nextElementSibling; 下一个元素节点 //<div class="item"> 2</div>
let previousElement=lastElement.previousElementSibling;  //<div class="item"> 2</div>
console.log(previousElement);
```
</script>

##### 节点的信息属性

nodeType nodeName nodeValue

```javascript
console.log("元素节点");
//nodeType nodeName nodeValue
console.log(box.nodeType);  //1
console.log(box.nodeName);  //DIV
console.log(box.nodeValue);  //null

//属性节点
let attrNode=box.attributes[0];
console.log("属性节点");
console.log(attrNode.nodeType); //2
console.log(attrNode.nodeName);  //class
console.log(attrNode.nodeValue); //box

console.log("文本节点");
console.log(firstChild.nodeType); //3
console.log(firstChild.nodeName); //#text
console.log(firstChild.nodeValue);

let comment=firstElement.nextSibling;
console.log("注释节点");
console.log(comment.nodeType); //8
console.log(comment.nodeName); //#comment
console.log(comment.nodeValue); //注释

console.log("文档节点");
console.log(document.nodeType);  //9
console.log(document.nodeName);  //document
console.log(document.nodeValue); //null
```
##### 添加元素

<body>

```javascript
<div class="box" title="item1">
</div>
<span></span>
```
</body>

​	document.createElement(标签名); 创建元素

​	设置元素属性

​	a.appendChild(b)  将b元素插入到a元素的内容之后   


```javascript
let box=document.querySelector(".box");
let divEle=document.createElement("div");
// console.log(divEle);
divEle.style.cssText="width:100px;height:100px;background:yellow";
box.appendChild(divEle);

插入的可以是已有的也可以是未定义的
let item=document.querySelector("span");
box.appendChild(item);
```


```javascript
let box=document.querySelector(".box");
let item1=box.firstElementChild;
let item3=box.lastElementChild;
let newdiv=document.createElement("div");
newdiv.className="item";
newdiv.innerHTML="4";
// box.appendChild(newdiv);

//a.insertBefore(b, c); //把b元素插入到a的子元素c前面
box.insertBefore(newdiv, item1);
box.insertBefore(newdiv,item3);

//createDocumentFragment() 创建一个文档片段
let f=document.createDocumentFragment();
for(let i=0;i<100;i++){
	let newdiv=document.createElement("div");
	newdiv.className="item";
	f.appendChild(newdiv);
}document.body.appendChild(f);

//a.replaceChild(b, c);//把a中的c元素替换为b元素
box.replaceChild(newdiv,item3);

//a.removeChild(b); 把a的子元素b移除掉
box.removeChild(newdiv);

//传址
let obj={name:"zhangsan"};
let obj2=obj;
obj2.name="lisi";
console.log(obj.name);
//传值
let a=1;
let b=a;
b=2;
console.log(a);
//a.cloneNode(true) 克隆一个a对象  内加true是克隆全部
let newbox=box.cloneNode(true);
document.body.appendChild(newbox);
```
### 二十二、事件流

> 当我们触发每个元素身上的事件的时候 当前元素的所有前辈元素 一直到整个页面 都会按照特定的顺序来响应这个事件  这种事件传播的方式叫做事件流。

##### 1.冒泡型事件流

> 默认存在的事件流，不需要特定的事件去触发

2.捕获型事件流

> 需要通过特定的方式触发   添加事件监听 第三个参数  设置为true

捕获型事件流在触发之后还是会进行冒泡的

##### 3.阻止浏览器默认行为

e.stopPropagation();

out   toElement

同步 异步执行代码     等的形式叫事件循环机制

##### 4.事件委派

e.target  目标、直接 事件源 最开始触发事件的元素

box.onclick=function(){

​	let target=e.target ;

​	if(target.className==="items"){

​	}

}

### 二十三、客户端存储【3.16】

##### 1.cookie

​	特点：1.保存数据量比较小 4kb 20 键值对

​	2.cookie 就是浏览器保存在硬盘中的一个文件

​	3.默认的保存时间是一次会话 但是可以保存任意长的时间

​	4.每一个网站都会保存自己单独的cookie文件

​	5.每一个浏览器会单独保存自己的cookie文件

​	6.同源策略  (协议 域名 端口号 完全一致)

##### 2.如何使用

document.cookie

浏览器--检查元素-->application 



document.cookie="name=zhangsan; expires="+date.toGMMMMMTString();

##### 3.localStorage sessionStorage

特点：1.保存的数据量比较大 5mb-10mb

​	2.localStorage 保存永久性的数据  sessionStroage 只能保存一次会话的数据

​	3.操作比cookie要方便很多

4 5 6均相同

##### 4.// 	window.localStorage

​	//设置

   localStorage.name="zhangsan";
​	localStorage.setItem("age",17);
​	localStorage["sex"]="男";
​	//获取
​	console.log(localStorage.name);
​	console.log(localStorage["age"]);
​	console.log(localStorage.getItem("sex"));
​	//删除
​	// localStorage.removeItem("name");
​	//清空
​	// localStorage.clear();
​	//遍历
​	console.log(localStorage.key);
​	for(let i=0;i<localStorage.length;i++){
​	    console.log(localStorage.key(i));
​	}

##### 5.

```javascript
localStorage.num=true;
let arr=[];
localStorage.date=arr;//toString
console.log(localStorage.date);
//ES5 新增对象 JSON 内置的对象 Math
//JSON.parse() 将字符串格式转化为对象
var str=`{"name":"张三"}`;
console.log(JSON.parse());
let obj={name:"zhangsan" };
console.log(JSON.stringify(obj));//对象转化为字符串

//不能直接存对象
let obj2=JSON.parse();//转化为对象
```
### 二十四、BOM 浏览器对象模型

window    history	 location 	screen	 document	 navigator

#### window 

##### 1.属性

screenleft    screenTop  火狐不能识别

screenX    screenY    

innerWidth  

innerHeight

localStorage

sessionStorage

top   访问父窗口的window对象

##### 2.方法

alert()   

prompt() 弹出输入框 请输入

confirm() 判断执行操作与否   

 setInterval     clearInterval ()     

getComputedStyle()获取任意元素的css属性

setTimeout(function(  ){ },3000)        clearTimeout

eg：	let st=setTimeout(function(  ){ },3000)  ;

​		 clearTimeout(st);

window.onpopstate  监测当前的变化

#### window.screen

#### window. navigator  

​    vender可以判断浏览器类型

#### history

##### 1.属性

history.length  表示当前浏览器保存了几条内容

history.state

##### 2.方法

forward() 前进

back()  后退

go(1)     前进一次   任意跳转  

 go（-1）后退一次

 go(0) 刷新

pushState({		},"	","xx.html")   在历史记录中添加一条新地址

​		     状态值  类型

replaceState({		},"	","xx.html") 直接替换当前的地址

#### location

##### 1.http://。。。。

##### 2.URL 统一资源定位符  

URI  统一资源标示符

URI包括URL 

http   https   协议

localhost  www.github.com    www.news.baidu.com    域名 

：63342   端口号   80   

/LOG/03.12..../xx.html    路径

？a=b&c=d&e=f    查询字符串

\#aa        锚链接  hash  

##### 3.属性

http  tcp  ip 

location.protocol        协议

location.hostname        localhost 域名

location.port   端口号

location.host   域名+端口号

location.pathname 

location.search  查询

location.hash  锚链接

location.herf   完整的URL

所有的这些属性都是可以设置的

```javascript
location.assign(".html");// 加载新页面  和正常点击a链接效果一样  有历史记录
location.replace("");// 加载新页面 替换 不产生历史记录
location.reload();//重新加载当前站点的资源
```
# 贰（一）jQuary

> js  ECMAScript  DOM+BOM 使用js的语法操作浏览器和文档中的内容

#### 1.优点：

1）.兼容旧的浏览器

2）.简化语法

#### 2.获取元素

单一的元素 还是集合 操作方式是一样的

#### 3.特点：

强大的查询（获取）功能

隐式的循环

链式调用

jquery 1.5   ie6-ie8

jquery 2.x    不支持旧浏览器

jquery 3.x  不支持旧浏览器

原生对象==>jQuery      $(原生对象)

```javascript
//grtAttribute() 获取元素的某个属性 setAttribute()  ==>attr
let div=document.querySelector(".demo");
console.log(div.getAttribute("data-msg"));
div.setAttribute("data-src","fdgdfgdfgv");

console.log($(".demo").attr("data-msg"));
$(".demo").attr("data-src","fdgdfgdfgv");

$(".demo").removeAttr("ddata-msg");

$("input");
$("[name='aa']");
// $(":checkbox").prop("disabled",true);
$(":checkbox").prop("checked",true);
// $(":checkbox").prop("checked",true);
//textContent 只表示文字内容    ==> text()
console.log(div.textContent);
div.textContent="123";  //设置时整个内容都改变

console.log($(".demo").text());
$(".demo").text("<span>123</span>");

//value
console.log($(":checkbox").val());
```

```javascript
//css
//offsetTop  offsetLeft ==> offset//相对于文档的  position//定位的left top 本身的
console.log($(".demo").offset()); //始终是相对于文档的位置
console.log($(".demo").offset().top);

console.log($(".demo").position());//定位的left top 本身的

//scrollTop scrollTop()  scrollLeft  scrollLeft()
$(window).scroll(function(){
    console.log($(window).scrollTop());
})

//width
console.log($(".demo").width());//本身
console.log($(".demo").innerWidth());//+内边距
console.log($(".demo").outerWidth());//offsetWidth +border
console.log($(".demo").outerWidth(true));//+外边距
```

```javascript
console.log($===jQuery);
let div=$("div");
console.log($("p",div));
console.log($("<div></div>"));
console.log($("<div>"));
console.log($("<div class='one'>"));
// $(function(){
//
// })
// $(document).load(function(){
//
// })
// window.onload=function(){}
// document.createElement()
// document.createDocumentFragment()
// appendChild
// 外部插入
//append appendTo prepend prependTo
// let p=$("p");
// let p=document.querySelector("p");
// $("div").append(p);
// $("div").append("p");  //"p"
//html片段  原生对象 jQuery对象
// $("div").html(function(index,val){
//     return "<span></span><p>"+(index+1)+"</p>";
// })
//
// $("div").append(function(index,val){
//     return "<p>"+(index+1)+"</p>";
// })
// $("<div>").appendTo(".demo");

$("div").after("<span></span>");
$("div").after($("p"));
$("div").insertAfter("p");

//包裹
$("div").wrap("<section></section>");//给每个包裹一次
$("div").wrapAll("<section></section>");//把所有的包起来
$("div").unwrap();//去掉包裹 不需要参数
$("div").wrapInner("<b></b>");//里面进行包裹
$("div").replaceWith("<p></p>");
$("<p></p>").replaceAll("div");
$("section").empty();
$("section").remove();
$("section").detach();
$("section").clone().appendTo("body");//先克隆后追加
```

```javascript
$(":button").click(function(){
    // $(":button").hide(10000);
    $(".demo").show(3000,"linear",function(){
        $(this).css("backgrounf","blue");
    });
    //$(".demo").toggle(1000);
    // $(".demo").slideDown(1000);//展开
    // $(".demo").slideUp(1000); //收起
    // $(".demo").slideToggle(1000);//转换
    // $(".demo").fadeOut();//淡出
    // $(".demo").fadeIn(1000);//淡入
    // $(".demo").fadeTo(1000,0.5);// 时间  动画透明度
    // $(".demo").animate({width:500,height:500},1000);//自定义动画（属性 速度 函数）
    let obj={t:0};
    $(obj).animate({t:2018},{
        duration:1000,
        step:function(){
            $(".year").html(Math.ceil(obj.t));
        },
        complete:function(){
            $(".year").html(2018);
        }
    })
})
```

```javascript
$(".container").on("transitionend",function(){})
```

```javascript
$(".container").on("click",".item",function(){
    $(this).css("background","red");
})
```

事件委派

$(".container").on("click",".item",function(){

```javascript
$(this).css("background","red");
```
})

# 叁、php

## B/S browser/server  C/S client/server

* 服务器  

  电脑

计算机 接收、发送信息

服务器软件 接收请求  发送响应   相应的软件：apache 

### wampserver 集成的服务器开发环境

w windows 操作系统 mamp  lamp

a apache 服务器软件(语言)            完整的实现了http协议

m mysql  数据库服务

p  php    集成的后台开发语言  对于php解析的支持  apache当中有一个模块可以解析php

### nodejs 

app分类：

原生app    java    andrio    object-c  ios

webapp      运行固定的网页

hybird app 混合器 html+css+js+底层接口

微信小程序 类似于混合app

## ajax 名词

### 一、字面意思 

异步的asynchnorous 

 javascript 

and 

XML一种数据的交换模式  string/json

### 二、用途：

在不跳转网页的前提下，实现数据交互的一种技术 

普遍运用在当前网络应用中的一种技术

### 三、好处：

用户体验更好

### 四、用法：

```php
1.实例化ajax对象 
		let xhr=new XMLHttpRequest();//ie6+
       //new ActiveXobject("Microsoft.XMlHTTP")//ie6
2.进行参数的配置
3.发送请求
4.等待接收响应
5.接收响应的数据
6.根据响应的数据对页面进行对应的处理
```

##### 五、get  post的区别

1.get  发送的数据是以查询字符串的形式直接连接在地址的后面的

post  发送的数据是放置在请求的主体body里面的

2.post的安全性比get高

3.get的速度快于post

4.post处理的数据量要比get大很多（文件 图片）

get

```php
//2.进行参数的配置
xhr.open("get","sign.php?phone="+val);
//3.发送请求
xhr.send();
```

post

```php
  xhr.open("post","sign.php");
  xhr.setRequestHeader("Content-Type","application/x-www-form-urlencoded");
  xhr.send("phone="+val);
```

##### MIME类型 ：

```php
xhr.setRequestHeader("Content-Type:application/x-www-form-urlencoded");
```

text/html  text/css  text/javascript     文本

image/jpg   image/png   图片

application/x-www-form-urlencoded  表单数据

##### ajax 2.0

```php
xhr.responseType="text";//json document
xhr.onload=function(){   //ajax 2.0
    //5.接收响应的数据
    let r=xhr.response;
    //6.根据响应的数据对页面进行对应的处理
    if(r==="1"){
        h3.innerHTML="号码可以使用";
    }else{
        h3.innerHTML="号码不可以使用";
    }
}
```

##### ajax 1.0

```php
     xhr.onreadystatechange=function(){
            //open send 接收到数据
            //xhr.readyState 当前的状态值
            // 0 open之前
//            1  open完成
//            2 send完成
//            3 响应接收到
//            4 响应处理完成
            if(xhr.readyState===4){
                //判断当前的状态码
                if(xhr.status===200){
                    //responseText responseXML
                    let r=xhr.responseText;
                    console.log(r);
                }
            }
        }
```
服务器程序

后台语言 php jsp ASP NET

数据库 以文件形式保存   mysql   sqlserver

phpmyadmin 数据库操作界面



ajax 请求是不允许跨域访问的

同域  cookie localStorage..  同域原则 同源策略

协议   域名 端口号 完全一致同域



解决跨域问题：

1.在后台程序中设置允许访问跨域访问

2.借助后台程序去请求另一个后台程序的信息    require

3.jsonp   json with padding

用来指定当前后台是使用什么名称来接收的



在jquery里 把jsonp请求数据这种方式 也封装到$.ajax函数中 但是两者是没关系的

<script  src=" http://localhost/ "	></script>

1.script 也是发起网络请求接收响应的一种方式

2.script 标签发起请求是没有跨域的限制的

3.script 也可以请求其它类型的文件

4.请求回来的数据会默认按照js的语法运行

## 阶段

语法： 变量 常量 数据类型 运算符 流程控制 函数 数组 对象 

功能：对于文件的处理 对于图像的处理  对于数据库进行操作  生成动态网页

面向过程的方式完成应用的制作 网站

面向对象的方式 （MVC架构） 购物app

# 叁、PHP

## 一、wampserver

- window  mamp  lamp
- apache  服务器语言，（接收一些请求，发送响应），完整的实现了http协议
- mysql
- Php     apache当中有一个模块可以解析PHP

## 二、PHP语法

### 0、作品

1、表格login  表格验证插件  表格login 

### 1.学习流程

变量、常量、数据类型、运算符、流程控制、函数、数组，对象

对于文件的处理      对于图像的处理

对于数据库进行操作，生成动态网页

面向过程的方式完成一个应用的制作  网站

面向对象的方式（MVC架构）       购物APP

### 2、输出   echo var_dump

注释 //        /* */      #

```php
echo "123","456";//输出单个或者多个
print 444;//效率较低  不使用
echo "<br>";//可以输入标签
echo("00");//只可以输出一组
var_dump(1+1);//输出值的类型和值 是一个函数
```

### 3、语法

php ：Hypertext preprosser  超文本预处理器

### 4、、变量

* 所有的变量都不需要提前声明
* 每一个变量都必须以$开始
* 真正的名字的开始  是以 字母  _  开始的  后续可以跟字母 下划线  数字
* 严格区分大小写的（函数名是不区分大小写的）
* 长变量 用_来连接
* 命名一定要有意义

### 5、超全局变量

>  php内部定义好的 可以在任意位置访问到的变量

> 变量保存的都是数组

* $_GET 用来存放浏览器通过get方式发送的请求数据
* $_POST 用来存放浏览器通过post方式发送的请求数据
* $_REQUEST 用来存放浏览器发出的所有请求数据
* $_COOKIE 用来存放浏览器发出的所有cookie数据    浏览器
* $_SESSION 用来存放浏览器发出的所有session数据 服务器  要先session_start();
* $_ENV   用来保存当前服务器的环境数据
* $_FILES 用来存放浏览器发送的文件数据
* $_SERVER  用来存放当前服务器的基本信息
* $GLOBALS  用来存放所有的全局变量

```php
var_dump($_GET);//用来存放浏览器通过get方式发送的请求数据
var_dump($_POST);//用来存放浏览器通过post方式发送的请求数据
var_dump($_REQUEST);//用来存放浏览器发出的所有请求数据
var_dump($_COOKIE);//用来存放浏览器发送的所有cookie
var_dump($_SESSION);//保存当前服务器的session信息
var_dump($EVN);  //用来保存当前服务器的环境数据
var_dump($FILES); //用来存放浏览器的文件数据
var_dump($SERVER); //用来存放当前服务器的基本信息
var_dump($GLOBALS);//用来存放所有的全局变量
```

### 6.常量

> 声明是通过const或者是define函数

```php
const A=1;
var_dump(A);
define("PI",3.14);
var_dump(PI);
```

> 使用const语法结构定义 比用define函数快

> 如果是在类当中定义常量，只能使用const

> 常量不需要加$，并且常量都是全部大写的

### 7.魔术常量

PHP内部预先定义好或者自己直接生成的一些常量

```php
var_dump(__LINE__);   //当前代码执行的所在行的行号
var_dump(__DIR__);    //当前文件所在目录
var_dump(__FILE__);   //当前文件在计算机中的完整路径

function fn(){
    var_dump(__FUNCTION__);//当前代码所在函数的函数名
};
fn();

class Human{
    public function  __construct()
    {
        var_dump(__CLASS__);//当前代码所在类的名称
    }
    public function say(){
        var_dump(__METHOD__);//当前代码所在类及方法的名称
    }
}

$someone=new Human();
$someone->say();
```

### 8.关于变量常量的函数

php内部预先定义好的或者是自己直接生成的一些常量

> __LINE__   当前代码执行的所在行的的行号

> __DIR__      当前文件所在目录

> __FILE__     当前文件在计算机中的完整路径

> __FUNCTION__ 当前代码所在函数的函数名

> __CLASS__    当前代码所在类的名称

> __METHOD__   当前代码所在类及方法的名称
>
> ```php
>  ```php
> var_dump(__LINE__);
> var_dump(__DIR__);
> var_dump(__FILE__);
> function fn(){
>     var_dump(__FUNCTION__);
> }
> fn();
> class Human{
>     public function __construct()
>     {
>         var_dump(__CLASS__);
>     }
>     public function say(){
>         var_dump(__METHOD__);
>     }
> }
> $someone=new Human();
> $someone->say();
> ​```
> ```

### 9、关于变量常量的函数

* isset()   判断某个变量是否被定义  返回布尔值

* unset()  将某个变量变为空值

* defined() 判断某个常量是否被定义

  ```php
  var_dump(isset($aa));//false
  unset($a);
  var_dump(isset($a));//false
  var_dump(defined("A"));//false
  ```

### 10、数据类型

 8种数据类型 4种标量 2种复合类型 2种特殊类型

##### 1、标量：

> 整数类型   int    1   2   1000
>
> 浮点数   1.0
>
> 布尔值 boolean/
>
> 字符串 string " "   '    '

> - "  " 是可以识别变量的 用{}可以更加明确变量的位置

- 整数类形（整形）   int  1  2  11100

```php
$num=1;
var_dump($num); 
//int 1
```

- 浮点数     float    1.1     1.0

```php
$num=1.1;
var_dump($num);
//float 1.1
```

- 字符串     string    ""     ''

*""当中是可以识别变量的，用{}包裹更加明确变量的位置

```php
$str="hello world";
var_dump($str);
//string 'hello world' (length=11)

$str2="hello $str";
var_dump($str2);
//string 'hello hello world' (length=17)

$str2="hello {$str}sddede";
var_dump($str2);
//string 'hello hello worldsddede' (length=23)

$str2='hello $str';
var_dump($str2);
//string 'hello $str' (length=10)
```

- 布尔值   boolean      true    false

```php
$boo=true;
var_dump($boo);
//boolean true
```

##### 2、两种复合类型：

>  数组 arrary

>  对象 object

- 数组  array

```php
$arr=[1,2,3,4,5];
var_dump($arr);
//array (size=5)
//  0 => int 1
//  1 => int 2
//  2 => int 3
//  3 => int 4
//  4 => int 5
```

- 对象  object

```php
class Human{
    function __construct()
    {

    }
}
$obj=new Human;
var_dump($obj);
//object(Human)[1]
```

##### 3、两种特殊类型：

- null  一个用于占位的空值

```php
$bar=null;
var_dump($bar);
//null
```

- 资源   resource

通过函数引用和释放的一些特殊的数据，比如打开的文件，连接的数据库或者创建的绘图板

```php
$file=fopen("demo.html","rw");
var_dump($file);
//resource(3, stream)
```

### 12、和数据类型有关的函数

* ##### 1、gettype() 获取某个变量的数据类型

  * 1.0                  double
  * 1                      integer
  * " abv"               string 
  * true                   boolean
  * [1,2,3]               array
  * new Human;    object
  * null                     NULL
  * 资源                    resource

```php
echo gettype($num);
echo "<br>";
echo gettype(1);
echo "<br>";
echo gettype("qwe");
echo "<br>";
echo gettype(true);
echo "<br>";
echo gettype($arr);
echo "<br>";
echo gettype($obj);
echo "<br>";
echo gettype($bar);
echo "<br>";
echo gettype($file);
```

##### 2.判断

> is_integer()是否是整数型
>
> is_string()是否是字符串型
>
> is_bool()是否是布尔值
>
> is_double()是否是浮动型
>
> is_array()是否是数组
>
> is_object()是否是对象
>
> is_null()是否是空值
>
> is_resource()是否是为资源类型

```php
var_dump(is_integer(1));
var_dump(is_string("1"));
var_dump(is_bool(true));
var_dump(is_double(1.0));
var_dump(is_array($arr));
var_dump(is_object($obj));
var_dump(is_null($bar));
var_dump(is_resource($file));
```

##### 3、强制转换

* intval()   强制转换为数值类型   转换不了即为0
* floatval()   强制转换为浮点类型   （字符串为0  true和数组为1 资源为3 ）
  * boolval()  强制转换为布尔值     假值: 0    0.0 " "   "0" false  null	
* strval()   强制转换为字符串类型    （ true为1  false为空 ）:

```php
var_dump(intval("0"));//纯数字字符串的 为int数值 不是的则返回0"zac123"  0
var_dump(floatval(3));//字符串的则为0  true 数组 为1  resource为3
var_dump(boolval($file));//0 0.0 ""  "0"  false null  为false
var_dump(strval("abc"));//true (1) false(空)
```

4、运算符

> * * \+ \- \++ \-- / %   .

> * ```php
>   * \+ \- \++ \-- / %
>   ```
>
> > < >= <= == != === !==
>
> ```php
> += -= *= /= %= .=连接操作
> ```
>
> > $$ and  || or  !
>
> ()

##### 5、流程控制

> * if(){}  if(){}else{}   if(){}else if(){}
> * switch(){}
> * for(){}
> * while(){}
> * do{}while(){}
> * {} 左边{替换为：冒号 右边}替换为endif;endwhile;endfor;endswitch
> * 流程控制语句可以跟html混排
> * foreach(){}专门用来遍历数组的

```php
<?php if ($age<18):?>
<div>未成年</div>
<?php else:?>
<div>成年</div>
<?php endif;?>
<ul>
    <?php for ($i=0;$i<10;$i++):?>
    <li><?php echo "$i"?></li>
    <?php endfor;?>
</ul>
```
### 13、函数

* 函数不是一种数据类型 就是一种语法结构

* 函数名的命名规范  函数不能被重新声明  

* 函数名只能以字母或者下划线开始  后续可以跟字母 数字 下划线_

* 可变函数  用变量赋值为函数名 这个变量可以被直接调用

* 如果函数定义了行参并且没有默认值  我们必须传递实参

  * 定义函数行参的默认值 直接在行参后=默认值


  * 如果函数有默认值的行参 要放置到无默认值的后面

* 如果没有定义返回值  函数运行结果为null

  * 定义返回值使用 return  $行参

* 全局变量在函数内部是不能被直接访问到的

  * 可以通过$GLOBALS这个数组来进行访问

  * 通过global关键字进行声明 声明之后就可以使用了

    ```php
    $dj=10;
    function fa(){
    	var_dump($dj);//错误
    //    var_dump($GLOBALS["dj"]);  //解决1   
        global $dj;                  //解决2
        var_dump($dj);
    }
    fa();
    ```

```php
function fn(){
    echo "这是fn";
}
function fn1(){
    echo "这是fn1";
}
$f=function (){echo "2";};
fn();
$f();
$foo="fn1";
$foo();


function fn3($num){}
fn3(1);

function fn3($b,$a=1){}
fn3(2);

function fn3($b,$a=1){}
$bar=fn3(1);
var_dump($bar);//null
```

* 所有函数都拥有全局的作用域

### 14、函数操作有关函数

* function_exists      判断函数是否存在   返回布尔值
* func_get_args        获取所有实参
* func_get_arg（n）获取第n个实参
* func_num_args     获取实参的个 数

```php
$a=function_exists("fa");
var_dump($a);//false

function fna(){
    var_dump(func_get_args());// 1  2  3  4  5
    var_dump(func_get_arg(0));//1
    var_dump(func_num_args());//5
}
fna(1,2,3,4,5);
```

### 15、数组

* 可以通过[]    也可以通过arrary() 
* 数组分为 索引数组 和关联数组 （类似于js中的对象）
  * 两种数组的写法可以合并

```php
$arr=[1,2,3,4,5];
$arr2=array(1,2,3,4,5);
var_dump($arr,$arr2);
var_dump($arr==$arr2);

$person=["name"=>"zhangsan","age"=>"18","sex"=>"man"];关联数组   索引数组是下标为0  1  2  3
var_dump($person);
```

* count() 用来计算当前数组的长度

### 16、session

* session  会话
* php session  和js sessionStorage完全没有关系
* 目的：让服务器能够识别当前正在访问的是哪一个浏览器
* 原因：因为HTTP协议是一种无状态的协议
* 浏览器向服务器发送数据的时候会自动的把cookie发送
* session_start（）；开启session
  * 判断当前发送过来的cookie当中是否包含sessionid
  * 如果没有 服务器就会控制当前浏览器在cookie当中自动生成一个sessionid的数据
  * 如果有  就会把当前这个sessionid对应的信息放置到$_SESSION这个数据当中
* session在服务器的保存有多种方式  文件 内存 数据库
* 在一个文件中只能有一个session_start（）

### 17、对象

* 在php能够控制每一个属性和方法的可访问性
  * private 私有的 只能在当前类中被访问到
  * protected  受保护的   只能在当前类以及继承了当前类的子类当中被访问到
  * public 公开的  能够在类的内部和外部都能被访问到

> 在类当中定义一个常量 会被当中当前类的属性来看待 实现访问是通过类的类名::属性名

> 类的成员可当做实例化对象的属性来访问

*  const 类的常量属性  static 类的普通属性   这两都是类的属性

* 函数的默认的访问权限  public

* 在类的内部可以通过$this实现对于当前对象的引用

* 在类的内部 构造函数是function __constructor(){}

* 在构造函数中或者是任意的方法中或者是实例化对象之后 都可以给当前对象添加属性 添加的属性默认都是public

  ​

  ```php
  class Human{
    function say(){
    	$this->arm=2;
    }
  }  
  $obj=new Human(23);
  $obj->say();
  $obj->legs=2;
  var_dump($obj);//  1
  ```

* 在类内部访问自己的属性是通过self::属性名

  ```php
  class Human{
    static $attr=1;
    function say(){
      echo self::$attr;
    }
  }  
  $obj=new Human(23);
  $obj->say();
  var_dump($obj);//  1
  ```

* 继承通过extends

* 重写构造函数需要通过parent::__construct调用父类的构造函数

# 肆、MySQL

### 1、数据库 DataBase

- 数据库

  > 计算机当中提供的存储数据的一种机制

-  SQL

  > 结构化查询语言

- MySQL

  > 数据库管理语言中的一种

- phpMyAdmin

  > 图形化的mysql操作界面  形式是以wed网页存在

#### 2、操作数据库

- cmd mingling  命令行

- ctrl +k  清空命令行

- 进入数据库

  > mysql -u root -p   不写分号

- 查看当前所有的数据库

  > show databases;   分号

- 创建一个数据库test

  > create database test;

- 删除某一个数据库test

  > drop database test;

- 进入某个数据库 test

  > use test;

- 显示当前数据库的表

  > show tables;

- 新建数据表class

  > create table class  (cid int primary key auto_increment not null,cname varchar(10) not null, croom varchar(10) not null ) engine=innodb default charset=utf8;  不写分号 点击确定 只是表示换行 

- 删除数据表clas

  >  drop table clas

- 插入数据

  > insert into class(cname,croom)values('WUIW1711','0203');
  >
  > insert into class()values(2,'WUIW1711','509');
  >
  > * 插入两条数据  逗号
  >
  > insert into class(cname,croom)values('WUIW1711','0203').('WUIW1711','0203');

- 删除数据

  > delete from class where cid=4;

- 修改数据

  > update class set croom='508' where cid=2; 
  >
  > * 修改多个字段
  >
  >   >  update class set croom='508',cname='WUIW1711-1'  where cid=2; 

- 表格内容的增加

  > alter table student add cld int not null;

- 单表查询数据

  * 无条件的查询所有的数据

    > select * from class;

  * 只查询某个字段

    > select sname from class;

  * 查询多个字段

    > select sname,ssex from class;

  * 指定从某个表中查询

    > select class.cname,ssex from class;

  * 给某个字段起别名

    > select cname as name from class;

  * 在查询的时候使用函数 sum count max min avg    无条件的查询 加条件用 where

    > * 查询年龄年龄之和
    >
    >   > select sum(sage) as total from student;
    >
    > * 查询所有的数
    >
    >   > select count(*) as number from student;
    >
    > * 查询最大的年龄
    >
    >   > select max(sage) as oldset from student;
    >
    > * 查询年龄最大的  名字和年龄
    >
    >   > select sname,sum(sage) as total from student;
    >
    > * 查询平均年龄
    >
    >   > select avg(sage) as average from student;
    >

  * where  对于查询结果进行筛选  = >  <  >=  <=   and between and  or  like

    > * select * ffrom student where sname='小红';
    > * select * from student where sage>18;
    > * select * from student where sage>18 and ssex='man';
    > * select * from student where sage>18 or ssex='man';
    > * select * from student where sname in ('小红','小王','小花');范围在（）里面
    > * select * from student where sname  like'小%'; %任意字符 任意长度

  * order by   asc 升序   desc 降序

    > * select * from student order by sage
    > * select * from student order by sage desc
    > * select * from student where ssex='man' order by sage ;

  * limit 10,3  从第10条开始取5条  限制条件

    > * select * from student limit 0,3;
    > * select * from student where ssex='man' order by sage desc limit 0,2;

  * group by  对于查询结果进行分组 一定是结合查询函数结合来使用的

    > * select cid,count(*) as num from student group by cid;
    > * select cid,count(*) as num2 from student where ssex='man' group by cid order by num2;

  * 查询子句 where |group by|having| order by|limit

  * having   一定是和group by 结合使用   分组之后的结果进行筛选

    > select cid,count(*) as num from student  group by cid having num>2;

    ​

- ##### 连表查询

  * 连表查询

    >  select * from student,class  where student.cid=class.cid;

  * 连表选择性查询

    >  select student.*,class.cname from student,class  where student.cid=class.cid;

  * 分组连表查询

    > select student.cid,count(*)as num,class.cname from student,class  where student.cid=class.cid group by student.cid;

    > select s.cid,count(*) as num,c.cname from student as s,class as c  where s.cid=c.cid group by s.cid; 
    >
    > 在from后面给表起别名 并把整条语句换别名显示  效果一样

  * ​

    > ​

- 视图

  * 新建视图message 包含 学生表的sid sname ssex

    >  create view message as select sid,sname,ssex from student;

  * 新建视图studentclass 包含学生表的全部和班级表的班级名称和教室

    > create view studentclass as select student.*,class.cname,class.croom from student,class where student.cid=class.cid;

  ​

- 练习 

  >  create database clothes 创建数据库;   use clothes;

  * 1、创建商品分类表  type   

    >  create table type  (tid int primary key auto_increment not null,tname varchar(10) not null ) engine=innodb default charset=utf8;

    * tid 分类id

    * tname 分类名称

      > ​

  * 2、向分类表中添加数据

    >  insert into type(tname)values('外套'),('裤子'),('鞋'),('其他');

    * 外套 裤子 鞋  其他

  * 3、创建商品表 goods    

    >  create table goods  (gid int primary key auto_increment not null,gname varchar(10) not null,gprice float(5,2) not null,gnumber int(10) not null,tid int(10) not null ) engine=innodb default charset=utf8;

    * gid   商品id
    * gname  商品名称
    * gprice 商品价格
    * gnumber  商品库存
    * tid 所属分类

  * 4、向商品中添加数据

    > insert into goods(gname,gprice,gnumber,tid)values('外套a','99','1000','1'),('外套b','199','200','1'),('裤子a','205','300','2'),('裤       子b','49','500','2'),('鞋a','56.9','3000','3'),('鞋b','36.5','1000','3'),('其他a','89.9','600','4'),;

  * 5、select * from goods order by gprice asc;                                                                      查询所有商品 按价格升序

  * 6、select * from goods order by gprice desc limit 0,3;                                                    查询价格最高的三个商品

  * 7、select sum(gnumber) as numtotal from goods;                                                          查询所有商品的库存总量

  * 8、select tid,avg(gprice) as avgprice from goods group by tid;                                       查询每种分类商品的平均价格

  * 9、select * from goods order by gid desc limit 0,1;                                                          查询最后一个添加的商品

  * 10、select goods.gname,type.tname from goods,type where goods.tid=type.tid;     查询商品的名称 以及分类名称

  * 11、select * from goods where tid=1;                                                                                 查询某个分类下的所有商品

  * 12、select tid,sum(gnumber) as tnumtotai from goods group by tid;                           查询每个分类的库存总量

  * 13、select * from goods where tid in(1,2) and gprice<200;                                查询价格在200以下的外套和裤子的商品

  * 14、select * from goods where gname like '%a';                                                               查询名字中包含a的商品

# web 全栈开发

1、背景和目的

2、分析     

​	1）需求分析

​       2）可行性分析      

​      3）技术分析    php+mysql    nodejs  express  / htm+css+js   /reactjs   /vuejs

3、设计

​	1 )   功能模块设计

 		功能模块图

​       	2）流程设计

​		流程图

​	3）数据库设计

​		E-R图  用例图   数据字典

​	4）文件架构设计

4、实现

​	搭建数据库

​	完成后台功能模块编写

​	完成前台功能编写

5、测试

# 伍、mvc

#### 1、mvc

> 对于软件的一种架构方式

m  model 模型  《——》  数据模型 和数据库对接

v view 视图        —— ---》  呈现在浏览器中的内容

c controller 控制器   ——完成中间的交接工作

#### 2、单页面入口	

> 不论我们当前是在进行前台展示还是后台管理 我们始终访问的是一个页面

#### 3、路由

> include   指定当前有哪些文件要加载扫我们当前入口文件执行

#### 4、模板引擎

> 让我们能够在html当中方便的执行一些php代码的一个工具，

框架  thinkphp  larva  

二次开发  内容 phpcms  论坛 discus  购物 ecshop  shopnc ....

# 陆、node.js 

### 一、原生开发

PHP的框架：thinkphp、larva……

二次开发：大部分是开源的（免费的），并不是偷懒、类似于 内容类型的phpcms，论坛类型的 discus，购物ecshop，shopnc……

### 二、nodejs

PHP是因为后台有对应的Apache服务器，所以可以被接收；而js是在浏览器，传到服务器里，在服务器里是不能直接运行js的；是通过nodejs来执行js的

#### 1、概念

>是一个服务器端的JavaScript运行环境

> 基于google浏览器v8引擎的封装  
>
> 并且还添加了很多其他的 功能 比如 文件操作 服务器软件搭建 

#### 2、Commonjs

Commonjs是JavaScript模块化的一个标准。（进行大型的开发必须得有模块化）；nodejs是Commonjs模块化标准的实现

#### 3、模块

>  nodejs 应用由模块组成的 在node中 一个文件就是一个模块

 文件类型3种

* js 解释执行
* json 会通过JSON.perse() 转化之后执行
* node  会调用对应的处理器进行处理

#### （1）、模块的划分

*   内置（核心）模块  在nodejs 启动的时候自动加载到程序当中的一些模块  比如 http  fs   url
*   文件模块  需要指定对应的路径来进行加载的一些模块

#### （2）、模块的使用 

* require  加载引入一个模块
* module.exports  定义当前模块导出的内容     
* exports  对于module.exports 的一个引用  
* 如果要引入的是一个js文件 可以不加后缀
* 每一个模块内部的属性和方法 都是不暴露的  需要暴露的话 module.exports导出
* ​

#### 2、require

* require  可以接收的参数有四种
  * 内置模块 直接写模块名字 引入 
  * 相对路径引入文件模块
  * 通过绝对路径引入文件模块
  * 通过直接写模块的名字来引入文件模块（通过npm install 下载安装的包会放置在当前文件夹下的node_modules文件夹  没有会自动创建）
    * 会在当前文件夹的node_modules文件夹中进行查找
    * 如果找不到 会继续去找上一级目录在上一级目录的node_modules文件夹中进行查找
    * 一直找到根目录

#### 3、包

* 包 能够完成某个功能的集合  集合是由一系列的模块组成
* package.json   用来描述和定义当前包的一些信息
  * main  表示当前包的入口在哪里
* 版本号 3位  x.y.z
  * z  小的修改   比如修复了一些bug
  * y   大的变动  比如添加了一个功能   会向下兼容
  * x   大的版本更新    比较多的删减  不会兼容低版本

（1）、npm  nodejs  package  manager  nodejs的包的管理工具

* 发布自己编写的包
* 下载别的开源的包
* 更新
* ....

#### 4、install/i   下载安装

* npm install   安装当前package.json 包含的所有依赖文件  然后遍历每一个安装的包 的package.json 再去下载它们的依赖文件
* npm install md5-node 安装一个
* npm install md5-node jquery bootstrap  安装多个
* npm install less -g 全局安装  
* npm install jquery@1.11.3 选择版本进行安装
* npm install jquery@lastest 选择最新版进行安装
* npm install md5-node --save   包会被添加到依赖当中
* npm install md5-node --save -dev    包会被添加到开发依赖当中

#### 5、npm init  初始化

* npm init
* npm init --yes

#### 6、依赖关系

dependencies

* 当前项目的依赖
* 在安装的时候加上--save，这个包会被添加到依赖当中,优点就是，加上save后传项目的时候就不用再传递node_modules，只用拷贝package-lock.json这个包就行，控制器就会直接执行里边的依赖。

devDependencies

* 开发过程中的依赖

### 三、fs系统文件

#### 1.文件

```
//stat判断当前资源是一个文件还是一个文件夹
// fs.stat("demo.txt",function (err,r) {
//     if(err) throw err;
//     // console.log(r.isFile());//判断是文件吗？
//     // console.log(r.isDirectory());//判断是文件夹吗？
// });
// 第一个参数文件路径,第二个参数是回调函数,回调函数的一个参数是表示错误，第二个表示结果。

//同步的方法就是在异步的后边加Sync就好
// let r=fs.statSync("demo.txt");//让stat成为同步判断
// console.log(r.isFile());//判断是文件吗？
// console.log(r.isDirectory());//判断是文件夹吗？

//2.exists判断某个资源是否存在
//es6中用箭头函数替换回调函数,左边是条件，右边花括号是结果
// fs.exists("demo.txt",(r)=>{//异步判断方法
//     console.log(r);
// });
// let res=fs.existsSync("demo.txt");//同步判断方法
// console.log(res);
//3.读取某个文件的内容
// fs.readFile("demo.txt","utf8",(err,data)=>{
//     if(err) throw err;
//     console.log(data);
// });
// let filecontent=fs.readFileSync("demo.txt","utf8");

// 4.writeFile向某个文件中写  如果文件已经存在则覆盖
// fs.writeFile("output.txt","hello",(err)=>{//会自动创建output.txt
//     if(err) throw err;
//     console.log("写入完成");
// });
// let writeFile=fs.writeFileSync("demo.txt","hello");

//5.appendFile向某个文件中追加内容
// fs.appendFile("demo.txt","world",(err)=>{
//     if(err) throw err;
// });
// let appendFile=fs.appendFileSync("demo.txt","world");

//6.rename 重命名
// fs.rename("haha.txt","demo.txt",(err)=>{
//     if(err) throw err;
// });
// let rename=fs.renameSync("haha.txt","demo.txt");

//7. unlink删除某个文件
// fs.unlink("demo.txt",(err)=>{
//     if(err) throw err;
// });
```

#### 2.文件夹

```
let fs=require("fs");
//1.mkdir创建文件夹，不能重复创建，不允许直接创建二级文件，只能直接创建一级文件夹。如果想直接创建二级文件夹，需要安装npm i mkdirp,就可以直接创建二级文件夹
// fs.mkdir("test",(err)=>{
//     if(err) throw err;
// });
//加载第三方模块后直接创建二级文件夹
// let mkdirp=require("mkdirp");
// mkdirp("test/aa",(err)=>{
//     if(err) throw err;
//     console.log("创建成功");
// });
//如果不想加载第三方模块，还要直接创建二级文件夹，就要把创建的方法都写同步方法。
// fs.mkdirSync("test");
// fs.mkdirSync("test/aa");

//2.readdir   读取某个文件
// fs.readdir("test",(err,result)=>{//参数1文件夹名称，参数2回调函数
//     if(err) throw err;
//     console.log(result);//结果为数组[ 'aa', 'css', 'index.html' ],数组包括每个文件夹的名字。
// });
// let data=fs.readdirSync("test");
// console.log(data);//结果为数组[ 'aa', 'css', 'index.html' ]

//3.重命名和文件一样

//4.rmdir删除文件夹  删除条件必须是空文件夹才能删除
// fs.rmdir("test/aa",(err)=>{
//     if(err) throw err;
//     console.log("删除成功")
// });
// fs.rmdir("test",(err)=>{
//     if(err) throw err;
//     console.log("删除成功")
// });
// let rmdir=fs.rmdirSync("test/aa");
// console.log(rmdir);//同步删除   结果为undefined

//对于文件的重命名
// fs.readdir("docs",(err,data)=>{
//     if(err) throw err;
//     // console.log(data);//[ 'a.txt', 'b.txt', 'c.txt' ]
//     data.forEach((name,index)=>{
//         // console.log(name);
//         let fullpath="docs\\"+name;
//         fs.renameSync(fullpath,"docs\\doc"+(index+1)+".txt");
//     });
//     console.log("修改成功");
// });

//合并文件
fs.readdir("docs",(err,data)=>{
    if(err) throw err;
    let str="";
    data.forEach((name,index)=>{
        let fullpath="docs\\"+name;
        let content=fs.readFileSync(fullpath,"utf8");
        str+=content;
        // fs.unlinkSync(fullpath);//合并完成后就删除每个内容
    });
    fs.writeFileSync("docs\\output.txt",str);
    console.log("合并成功");
});
```

#### 3.拷贝

```
const fs=require("fs");
// copy("demo.txt","index.txt");
copySync("demo.txt","index.txt");

//异步拷贝
function copy(src,target) {
    fs.exists(src,function (r) {
        if(r){
            fs.readFile(src,"utf8",function (err,data) {
                if(err) throw err;
                fs.writeFile(target,data,function (err) {
                    if(err) throw err;
                    console.log("拷贝完成");
                })
            })
        }else{
            console.log(r);
        }
    })
}
//同步拷贝
function copySync(src,target) {
    let exists=fs.exists(src);
    if(exists){
        let data=fs.readFileSync(src,"utf8");
        fs.writeFileSync(target,data);
        console.log("拷贝完成");
    }else{
        return false;
    }
}
```

#### 4.路径

```
let path=require("path");
//join 拼接不同的路径片段
let newpath=path.join("web","css","index.css");
let newpath1=path.join("web","\\css","index.css");
let newpath2=path.join("web","\\css","./index.css");
//以上三种结果都为web\css\index.css
// console.log(newpath);//结果web\css

//__dirname     __filename  都是绝对路径
// console.log(__dirname);//D:\wamp\www\5_3   当前文件所在文件夹的绝对路径
// console.log(__filename);//D:\wamp\www\5_3\path.js     当前文件的绝对路径
// console.log(path.join(__dirname,"docs"));//D:\wamp\www\5_3\docs

//reslove  专门把当前的路径转化为绝对路径用的
// console.log(path.resolve("docs"));//D:\wamp\www\5_3\docs直接获取docs的绝对路径
// console.log(path.resolve("docs\\output.txt"));//D:\wamp\www\5_3\docs\output.txt直接获取docs下的output绝对路径

//isAbsolute判断某个路径是否为绝对路径
// console.log(path.isAbsolute("docs"));//false
// console.log(path.isAbsolute(path.resolve("docs\\output.txt")));//true

//basename  extname
let p='D:\\wamp\\www\\5_3\\docs\\pouput.txt';
console.log(path.basename(p));//当前的文件名pouput.txt
console.log(path.extname(p));//文件的扩展名.txt
console.log(path.parse(p));//可以把当前路径转化为对象
// { root: 'D:\\',
//     dir: 'D:\\wamp\\www\\5_3\\docs',
//     base: 'pouput.txt',
//     ext: '.txt',
//     name: 'pouput' }
console.log(path.dirname(p));//当前路径的文件夹部分 D:\wamp\www\5_3\docs
```

### 四、http

#### 1.nodemon

路径：C:\Users\asus\AppData\Roaming\npm\node_modules\nodemon\node_modules\fsevents\node_modules'

每次写一次响应内容都要在控制器中执行一次，为了方便，安装一个包npm    inatall     nodemon   -g   --save    就可以不重复执行了。执行的代码四nodemon  http.js,这个nodejs会时时监听数据改变。

```
const http=require("http");//内置模块，不需要安装
const fs=require("fs");
const path=require("path");

//搭建服务器
// createServer()   返回一个server类,参数是一个请求的监听函数,在这个过程中会自动传递两个参数（实例化的两个类，1.http.IncomingMessage 类和2.http.ServerResponse 类）
const server=http.createServer(function (request, response){
    // console.log(request);
    //响应的内容用write写，内容格式为字符串或者为buffer，end表示响应结束
    //写内容方法1
    // response.write("hello");//write可以写多个
    // response.end();
    //写内容方法2
    // response.end("hello",()=>{
    //     console.log("当前响应完成");
    // });//响应内容也可以写在end中的第一个参数
    let url=request.url;
    if(url==="/favicon.ico"){
        response.end();
        return;
    }else if(url==="/index"||url==="/"){
        response.writeHead(200,{"Content-Type":"text/html;charset=utf8"});
        //200是状态码。
        fs.readFile(path.join(__dirname,"static","index.html"),function (err,data) {
            if(err){
                response.write("404 页面未找到");
            }else{
                response.write(data);
            }
            response.end();
        })
    }else if(url==="/login"){
        response.writeHead(200,{"Content-Type":"text/html;charset=utf8"});
        response.write("登录页");
        response.end();
    }else {
        response.writeHead(404,{"Content-Type":"text/plain;charset=utf8"});
        //上一行代码是为了解决下一行代码乱码的。第一个参数是返回的信息，第二给我参数是用来描述的，可以不写。第三个参数是响应头
        response.write("404 页面未找到");
    }
});
server.listen(8888,function () {
    console.log("服务器开启成功");
});//开启http监听连接，参数是要监听的端口，
```

#### 2.mime

mime可以根据不同的类型来加载不同的后缀名的文件。比如说在js中加载一个html文件，而html中有css的引入，不使用mime的话，则css是不会实现效果的，图片也是一样，图片就不会加载出来。只有HTML代码。没有样式。npm  install  mime

### 五、url

```
//对于整个路径的解析
const url=require("url");
let path="http://nodejs.cn/api/http.html?name=aa";
console.log(url.parse(path));

parse可以将path转换为一个对象
Url {
    // protocol: 'http:',    协议
    //     slashes: true,
    //     auth: null,
    //     host: 'nodejs.cn',
    //     port: null,
    //     hostname: 'nodejs.cn',
    //     hash: null,
    //     search: '?name=aa',
    //     query: 'name=aa',
    //     pathname: '/api/http.html',
    //     path: '/api/http.html?name=aa',
    //     href: 'http://nodejs.cn/api/http.html?name=aa' }

//处理查询字符串
// const qs=require("querystring");
// let query="name=zhangsan&age=17";
// console.log(qs.parse(query));
```

### 六、express

#### 1、概念

> 基于nodejs的简洁 快速 高效的web开发框架

> 进行pc端或者移动端web项目的后台开发

#### 2.文档：

​	express官网      http://www.expressjs.com.cn/guide/routing.html

#### 3、特点

> 一个express搭建的后台框架 就是由路由和中间件组成的

> express 并没有对于node进行二次的扩展 只是对于原生node进行封装 也就类似于js与jqury

#### 4、安装

cnpm install express --save

npm install express --save

### 七、路由

- 定义：路由就是服务器根据客户端请求的地址和方式，返回不同资源的方式
- send();发送数据的，是express特有的，发送的数据会在浏览器中呈现的。
- end();是原生nodejs的方法，也可以发送数据，也代表结束。
- use();是专门用来加载中间件的方法的，要使用中间件就必须用use方法。专门用来设置中间件的
- all();是一种特殊的路由方法，所有请求加载中间件的方法都要通过它。

```javascript
//all 执行完整匹配，use 只匹配前缀
app.use("/",function (req,res,next) {
    console.log("aaa");
    next();
});
app.all("/",function (req,res,next) {
    console.log("根路径的处理");
    next();//可以替换为res.end();
});
访问 / use 和 all 都会被调用；访问 /a 只有 use 被调用
```

- get、post、put....他们都是一样的作用，只是为了更好地识别这个方法到底是干什么的，和HTML中的div   header相似。

### 八、中间件

- 应用级中间件    没有挂载路径的中间件，应用的每个请求都会执行该中间件，有挂在路径的中间件，会执行特定的中间件

  ```javascript
  var app = express();

  // 没有挂载路径的中间件，应用的每个请求都会执行该中间件
  app.use(function (req, res, next) {
    console.log('Time:', Date.now());
    next();
  });

  // 挂载至 /user/:id 的中间件，任何指向 /user/:id 的请求都会执行它
  app.use('/user/:id', function (req, res, next) {
    console.log('Request Type:', req.method);
    next();
  });
  ```

- 路由级中间件

- 错误处理中间件

- 内置中间件  `express.static` 是 Express 唯一内置的中间件。它基于 [serve-static](https://github.com/expressjs/serve-static)，负责在 Express 应用中提托管静态资源。express.static(root, [options])

- 第三方中间件

### 九、模板引擎ejs

动态插入数据

模板引擎放置的目录是views

安装模板引擎：npm install ejs --save

ejs官网：https://ejs.bootcss.com/

```
app.set('view engine', 'jade');加载模板引擎模块
```



cookie      cookie  cookie-parser                                 https://www.npmjs.com/package/cookie-parser

session     session express-session                            https://www.npmjs.com/package/express-session

# 柒、Vue.js



#### 1、文本插值

文本插值     {{}}    v-html     v-text

* v-once   将不会被改变

```vue
<div id="app1" >{{message}}</div>   //hello
<div id="app2" v-html="content"></div>   //helloword
<div id="app3" v-text="text"></div>   //<h1>helloword</h1>

<div id="app1" v-once>{{message}}</div>   //不会被改变
<script>
var app=new Vue({
    el:"#app1",
    data:{
        message:"hello"
    }
});
  var app2=new Vue({
    el:"#app2",
    data:{
        content:"<h1>helloword</h1>"
    }
});
  var app3=new Vue({
    el:"#app3",
    data:{
        text:"<h1>helloword</h1>"
    }
});
 </script>
```

#### 2、指令

指令  v-bind:

* 特性 

  > 1、简写  :
  >
  > 2、可以写多个
  >
  > 3、在值当中也是可以写 表达式的

```vue
<div id="app3">
    <img v-bind:src="imgurl" alt="">
    <img :src="'http://'+imgurl" :alt="message">//值当中写表达式
</div>
<div id="app4" :class="className">hello word</div>
<div id="app5" :class="{underline:hasUnderline}">hello old
    <input type="button" value="toggle" v-on:click="toggle">
</div>
<script>
var app3=new Vue({
        el:"#app3",
        data:{
            imgurl:"99.jpg",
            message:"提示信息"
        }
    });
   var app4=new Vue({
        el:"#app4",
        data:{
            className:["one","two"],  //类名就会是两个one  two 
        }
    });
  var app5=new Vue({
        el:"#app5",
        data:{
            hasUnderline:false  //true  false两个值 true 设置的存在 false设置的不存在
        },
        methods:{
            toggle:function () {
                this.hasUnderline=!this.hasUnderline;
            }
        }
    });
</script>
```

#### 3、事件监听

v-on:   或者@

```vue
<div id="app5" :class="{underline:hasUnderline}">hello old
    <input type="button" value="toggle" v-on:click="toggle">
</div>
<script>
var app5=new Vue({
        el:"#app5",
        data:{
            hasUnderline:false
        },
        methods:{
            toggle:function () {
                this.hasUnderline=!this.hasUnderline;
            }
        }
    });
</script>
```

#### 4、条件与循环

条件与循环

1、条件

* v-show   v-if   显示与否 

```vue
<div id="app1" v-show="isShow" >helli</div>//v-show  true时显示 false时不显示 displace：none
<div id="app2" v-if="isShow" >helli</div>//v-if  true时存在 显示  false时html中就已经不存在了
<script>
var app1=new Vue({
        el:"#app1",
        data:{
            isShow:true
        }
    });
  var app2=new Vue({
        el:"#app2",
        data:{
            isShow:true
        }
    });
</script>
```

* v-if  v-else  v-else-if

  ​

```vue
<div id="app2"  >
    <input type="button" value="or" v-on:click="toggle">  点击一些显示的是v-if对的div的内容 再点击一下显示v-else的div的内容
    <div v-if="isShow">hellow</div>
    <div v-else>aaaa</div>     
</div>
<script>
var app2=new Vue({
        el:"#app2",
        data:{
            isShow:false
        },
        methods: {
            toggle:function () {
                this.isShow=!this.isShow;
            }
        }
    });
</script>
```

```vue
<div id="app3">
    <h3>订单状态</h3>
    <input type="button" value="切换" @click="change">
    <div v-if="state===0">未付款</div>
    <div v-else-if="state===1">已付款</div>
    <div v-else-if="state===2">配送中</div>
    <div v-else-if="state===3">配送完成</div>
    <div v-else>其他状态</div>
</div>                  点击切换按钮 五个内容依次显示 最终定格在其他状态
<script>
var app3=new Vue({
        el:"#app3",
        data:{
            state:0
        },
        methods: {
            change:function () {
                this.state++;
            }
        }
    })
</script>
```

##### 2、循环

```vue
<div id="app1">
    <ul>
        <li v-for="list in lists">{{list}}</li>
      <li v-for="list of lists">{{list}}</li>  //第一个名字与{{name}}相同  in/of  后面的参数与jS中的data的名字相同
    </ul>
</div>

<div id="app2">
    <ul>
        <li v-for="item in obj">{{item}}</li> //循环的是对象 这是其中的值的循环
        <li v-for="(val,key) in obj">{{key}}:{{val}}</li>// 这是键与值的循环  小括号中的第一个为值 第二个为键

    </ul>
</div>
<script>
var app1=new Vue({
       el:"#app1",
       data:{
           lists:[1,2,3,4,5,6]
       }
   })
    var app2=new Vue({
        el:"#app2",
        data:{
            obj:{name:"zhangsan",age:"17",sex:"fff"}
        }
    });
</script>
```

##### 3、表格的增删

```VUE
<table id="app3">
    <tr>
        <th>姓名</th>
        <th>年龄</th>
        <th>性别</th>
        <th>操作</th>
    </tr>
    <tr v-for="obj in studentData">
        <td>{{obj.name}}</td>
        <td>{{obj.age}}</td>
        <td>{{obj.sex}}</td>
        <td class="del" @click="del(obj.name)">删除</td>
    </tr>
    <tr>
        <td id="add" colspan="4" @click="add">+</td>
    </tr>
</table>
<script>
  var app3=new Vue({
       el:"#app3",
       data:{
           studentData:[{name:"zjangdan",age:18,sex:"man"},{name:"frsefr",age:7,sex:"man"},{name:"frgtr",age:50,sex:"man"}]
       },
        methods:{
           add:function () {
               this.studentData.push({name:Date.now(),age:"",sex:""});
           },
            del:function (name) {
                var data=this.studentData;
                data=data.filter(function (val,index) {
                    return name!==val.name;
                });
                this.studentData=data;
            }
        }
   })
</script>
```

##### 4、订单计算功能

```vue
<table id="app3">
    <tr>
        <td>选择</td>
        <td>名称</td>
        <td>单价</td>
        <td>操作</td>
        <td>数量</td>
        <td>操作</td>
        <td>价格</td>
    </tr>
    <tr v-for="good in goods" v-if="good.count!==0">
        <td><input type="checkbox" v-model="choose" :value="good.name"></td>
        <td>{{good.name}}</td>
        <td>{{good.price}}</td>
        <td @mousedown.prevent="del(good)" >-</td>
        <td>{{good.count}}</td>
        <td @mousedown.prevent="add(good)">+</td>
        <td>{{getprice(good)}}</td>
    </tr>
    <tr>
        <td colspan="7">{{choosestr}}</td>
    </tr>
    <tr><td colspan="7">总价：{{total}}</td></tr>
</table>
<script>
new Vue({
        el: "#app3",
        data: {
            goods: [{name:"苹果",price:20,count:1},{name:"香蕉",price:60,count:1},{name:"李子",price:85,count:1},{name:"西瓜",price:130,count:1},{name:"草莓",price:30,count:1},{name:"荔枝",price:30,count:1}],
            choose:[]
        },
        computed:{
            total: function () {
                var total=0;
                var goodsarr=this.goods.filter((v)=>this.choose.includes(v.name))
                goodsarr.forEach((obj)=>{
                    total+=obj.price * obj.count
                });

                return total ;
            },
            choosestr:function () {
                return this.choose.join("、");
            }
        },
        methods: {
            del: function (obj) {
                obj.count>0?obj.count--:"";
            },
            add: function (obj) {
                obj.count++;
            },
            getprice:function(obj){
                return obj.price*obj.count;
            }
        }
    })
</script>
```

##### 5、表单输入绑定

> 你可以用 `v-model` 指令在表单 `<input>` 及 `<textarea>` 元素上创建双向数据绑定。它会根据控件类型自动选取正确的方法来更新元素
>
> `v-model` 指令，它能轻松实现表单输入和应用状态之间的双向绑定

```vue
<script>
        //双向数据绑定
    new Vue({
        el: "#app1",
        data: {
            message: "hello word"
        },
        computed: {
            reverseMessage: function () {
                return this.message.split('').reverse().join('');
            }

        }

    });
</script>
```
#### 缺少好多

webpack

安装 npm install -g --save-dev webpack webpack-sli

默认配置文件夹在dist   控制器中执行webpack  --development  会在dist中生成main.js    是关于自己操作的src中的js文件的配置

 自己操作的文件夹为src    

建webpack.config.js作为配置

```js
let path=require("path");//地址
module.exports= {
    mode:"development",//开发版本
    entry:"./src/index.js",//入口的文件
    output:{
        path:path.resolve("./public"),
        filename:"index.js"
    },//出口的文件
    module:{
        rules:[
            {
                test:/\.css$/,                             //配置运行css需要的配置
                use:["style-loader","css-loader"]          //运行css需要安装这两个包
            },
            {
                test:/\.less/,                            //配置运行less需要的配置
                use:["style-loader","css-loader","less-loader"]   //运行less需要安装这san个包
            }
        ]
    }
};
```

构建工具 vuecli



# 捌、react

构建工具  create-react-app   官方推出的

安装 cnpm i  create-react-app  -g

创建项目：

```
create-react-app   test//项目名称
```



路由  react-router-dom





























































