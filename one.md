# 学习过程
## 前端基础
* 语言
> HTML4 HTML5 CSS2 CSS3 
* 技能
> PC端的网页布局  移动端网页布局  响应式布局 HTML5特性使用
## 前端进阶
* 语言 
> JavaScript (JS) jQuery 
* 技能
> ECMAScript5 ECMAScript6 BOM DOM AJAX使用 jQueryAPI  jQuery插件 
## 全栈基础
* 语言 
> PHP MySQL 
* 技能
> 面向过程的网站前后台搭建  MVC设计思想  基于MVC的框架搭建   框架下的项目开发  HTTP协议 模板引擎  
## 全栈进阶
* 语言
> Nodejs
* 技能
> Node基本使用  搭建服务器  express搭建服务器 VUE REACT 快速构建有丰富交互功能的网站页面 

## 其它
* markdown 
* sublime webstorm phpstorm 
* wamp
* git github  
* 服务器项目部署
* xmind

# HTML4

- 标签 div p pre ul li ol dl dt dd table tr td i em b strong img a input form textarea option select
- 属性 class  id   src title  alt 
- 表单 
  - type类型  text password radio checkbox button submit file hidden reset
  - 控件标签 input textarea select option 
  - 属性 value name disabled readOnly maxlength size cols rows multiple
  - form 属性  method action entype 

# HTML5

- 标签 
  - 语义化标签 header footer main section nav hgroup aside  time progress address 
  - 功能性标签 video audio canvas
- 属性 hidden draggable 自定义 data-
- 表单
  - type类型 email url date month week datetime-local color number range search 
  - 属性 placeholder autofocus required pattern autocomplete novalidate  
    - submit formaction formmethod formenctype
    - number/range  min max step 

# CSS2

- 选择器 
  - ".one" 类名选择器
  - "#aa"  id选择器
  - "div"  标签选择器
  - "div,p" 群组选择器
  - "*"    通用选择器
  - "div.one" "div#aa" 交叉选择器
  - "ul li" 后代选择器
  - "div>p" 子选择器
  - "div+p" "div~p" 相邻选择器
  - ":hover" ":link" ":active" ":visited" ":first-line" ":filrst-letter" 伪类选择器  
  - 优先级  !important style  交叉 后台>id>class>标签名>通用>默认样式>继承的样式
  - 权重 #one .two   .one>.two    
- 属性    
  - font-family 字体   多个 '微软雅黑','黑体'
  - font-size 大小  px  em rem
  - color  red #000 rgb()  (css3 rgba() hsl() hsla() transparent)
  - font-weight bold 数值 normal
  - font-style  itailc normal 
  - text-decoration   none underline...
  - text-align  center right left
  - line-height  垂直居中 
  - vertical-align 行内块级元素的垂直对齐
  - text-indent 文本缩进
  - width height   100px 50% 50vh 1rem auto
  - margin margin-left margin-right...  margin:0 auto;
  - padding 容器宽度高度
  - border  上下左右 样式 颜色 粗细  1px solid red    
  - background background-image background-color background-repeat background-position 图片精灵 background-attachment 
  - float 浮动  left right 
  - clear:both 清除浮动的影响
  - position 相对定位relative 绝对定位absolute 固定定位 fixed  静态定位 static 
  - left right top bottom z-index层级 
  - display none block inline inline-block  table table-row
  - overflow 超出部分的处理 overflow-x overflow-y
  - cursor pointer move

# CSS3

- 选择器

  - "[name]"  "[name=aa]" "[name^=aa]" "[name$=aa]" "[name*=aa]" 属性选择器
  - ":first-child" ":last-child"  "nth-child()" ":nth-last-child()" "only-child" 
  - ":first-of-type" ":last-of-type" ":nth-of-type()"  ":nth-last-of-type()" "only-of-type"
  - :before :after   content:""
  - :disabled :enabled :checked 
  - :root  :target 

- 属性

  - border-radius  圆角  (10px) (10px 20px) 椭圆(10px/5px)  (10px 20px/5px 10px) 
  - box-shadow offsetx offsety blur [size] color [inset] 
  - background-size cover|contain|100px|50%
  - background-clip border-box|padding-box|content-box
  - background-origin border-box|padding-box|content-box 
  - border-image-source
  - border-image-width
  - border-image-repeat
  - border-image-offset
  - outline 1px solid red;   
  - outline-offset 10px;
  - box-sizing border-box;  width 100px content padding border
  - column 
  - transition 过渡  （属性 时间 时间函数 延迟）
  - transform 转换 2d/3d
    - translate translateX translateY translateZ translate3d
    - rotate rotateX rotateY rotateZ rotate3d(1,1,1,45deg)
    - scale scaleX scaleY
    - skew skewX skewY
    - matrix()
  - transform-origin 
  - transform-style
  - perspective 景深
  - perspective-origin 
  - backface-visibility 背面是否可见
  - @keyframes 定义动画  百分比  from to 关键帧
  - animation：name time timing-function delay count direction play-state alternate
  - @media 媒体查询  响应式
  - @font-face 引入字体   iconfont
  - 弹性布局
    - display:flex;
    - 容器 flex-wrap flex-direction justify-content align-content align-items 
    - item flex-grow flex-shirnk order align-self

- 移动端布局

  - rem  
    1. 相对于html标签字体大小的相对单位 
    2. 在不同分别率下调整html字体大小
    3. JS脚本   媒体查询 
  - 百分比
  - vw vh 
  - 响应式        

- 响应式

  - 原理 @media 媒体查询
  - 栅格系统  bootstrap 

- 兼容性问题

  - 现代浏览器  user-select   caniuse  前缀 -ms- -moz- -webkit-
  - ie8以下 平稳退化   polyfill js脚本  ie8 js脚本
  - ie6兼容   

- 浏览器内核

  - IE trident CHROME webkit FIREFOX gecko  (360 QQ 搜狗 UC)

- 优化网页性能

  - 图片精灵
  - DATAURL  base64
  - 语义化标签
  - 图片质量  低  jpg  png
  - 布局结构 精简 清晰
  - 删除注释
  - 移动端 少用动画  css3  transform  

- 快速布局       

  - bootstrap

  - antd

  - 套模板

    ​     

​      

​        JavaScript

- ECMAScript
  - 语言特性：基于对象和事件驱动 解释型 松散型 语言
  - 数据类型：
    - 初始类型 数值 字符串 布尔值 undefined null Symbol  栈区 定长
    - 引用类型 对象（数组对象 函数对象） 堆区
    - why 内存    
  - var和let区别
    - var一直存在  let ES6中新增
    - var会被优先解析 let 不会
    - var 可以重复声明变量  let 不可以
    - var 全局声明的变量会自动添加为window对象的属性 let不会
    - let 是会识别块级作用域 var不识别
  - 运算符
    - ==只比较值是否相等  === 还要判断数据类型是否相同
    - 三元表达式   表达式1?表达式2:表达式3  
    - && || !  
      - window.aa&&aa()  if(window.aa){aa()}  
      - n=num||10     if(num){n=num}else{n=10}
  - 流程控制
    - 顺序结构 
    - 选择结构 if(){} if(){}else{}  if(){}else if(){}  switch(){} 
    - 循环结构 for(var i=0;i<10;i++){}  while(){}   do{}while()
    - for次数是固定 while不一定
    - break结束当前循环执行后续代码 continue 结束当前这一次循环 如果有下一次 继续执行
  - 函数 
  - 封装起来可以被重复使用的代码块
  - 接收参数 返回结果 return
  - 参数 形参 实参 
  - arguments对象 保存实参信息
  - 作用域 
    - 全局作用域 所有代码执行的环境
    - 局部作用域 函数内部  let const {}
    - 为什么 保护全局变量不受污染  命名更加方便
    - 作用域链  函数嵌套函数  自动形成一条作用域链 当我们访问某个变量 会沿着作用域链一直向上查找
  - 闭包   
  - 递归函数  函数内部自己调用自己   n维数组  对象拷贝 算法 合并排序 快速排序    
  - 回调函数  把一个函数作为另外一个函数的参数传递使用  单线程异步机制 函数  
- 数组
  - 方法 push() pop() unshift() shift() join() slice()  concat()  sort()  forEach() map() filter() some() every()  indexOf() lastIndexOf()  reverse() reduce() reduceRight()  find() findIndex()  fill() copyWithin() includes()    
- 字符串
  - 方法 charAt() charCodeAt() indexOf() lastIndexOf()  match(reg) search(reg) replace() toUpperCase() toLowerCase() slice() substring() substr() startsWith() endsWith() includes() trim()
- 对象
  - 属性和方法的无序集合
  - 类 具有相同或者相似属性的对象的抽象描述 类的具体化或者是实例化的结果就是对象  function(){} prototype 实现类      class extends 
  - new  Fn() 内部  
  - var obj={};
  - obj.__proto__=Fn.prototype;
  - Fn.call(obj);
  - this 
    - function fn(){console.log(this)}   //fn() window
    - obj={fn:function(){console.log(this)}}  //obj.fn() obj var f=obj.fn; f() //window  
    - fn.call(obj,1,2,3)  fn.apply(obj,[1,2,3]) 改变this的指针
    - var fn=function(){}.bind(obj)  fn()   

```javascript
    var a=1;
    var obj={
        a:2,
        fn:function(){
            return function(){
                     console.log(this.a)
            }
        }
    };
```

- 继承
  - prototype

```javascript
  function Human(){
    
  }
  Student.prototype=new Human();
  function Student(){
    
  }
```

- call/apply

```javascript
   function Human(){
    
   }
   function Student(){
      // Human.call(this)
      Human.apply(this)
   }
```

- ECMAScript6  2015 2016 2017
  - let变量 const常量
  - 块级作用域  {}  if(){} for(){}   
  - Symbol() 唯一值
  - 2**3幂运算  ...[1,2,3]  结果 1,2,3  扩展运算符 
  - `1+1=${1+1}` 模板字符串
  - let [a,b,c]=[1,2,3]; {name}={name:"zhangsan"} 解构赋值  
  - 参数的默认值 function fn(a=1){} 
  - setInterval(function(){},300) setInterval(()=>{},300) 箭头函数不会产生新的this和arguments对象
  - class  extends  super
  - Promise 
  - 模块系统  export  import        

# BOM

- BOM browser object model 浏览器对象模型 定义了如何通过js操作浏览器的各个部分
- window location history document screen navigator
- window 
  - 浏览器中js的全局对象 
  - 属性和方法   在任意
  - var function fn(){}
  - 属性 location history document screen navigator  
  - localStorage+sessionStorage  
  - alert() confirm() prompt() 
  - setInterval() setTimeout() clearInterval() clearTimeout() 
  - 动画 requestAnimationFrame() cancelAnimationFrame()  
  - getComputedStyle()
  - onload
- history
  - forward()
  - back()
  - go()
  - pushState() 添加一条历史记录    H5的方式
  - window.onpopstate()   react vue 
- location 
  - 协议 protocol https: // 域名 host cn.vuejs.org //端口号port :80 //path 路径 /v2/guide/index.html  / /index /index/main   //查询字符串 search ?name=asda&as=as //锚链接 hash #        href获取 设置
- replace()  assign() reload() 
  ​    

# DOM

- document object model 文档对象模型 定义了如何通过js操作文档的各个部分
- 属性 cookie  images forms links all  body head
- 方法 
  - querySelector  querySelectorAll 
  - createElement  createDocumentFragment             
- 元素对象 标签对象 
  - 属性 innerHTML textContent className id style  classList(add() remove() toggle() contain()) offsetWidth offsetHeight  offsetLeft  offsetTop scrollTop scrollLeft parentNode childNodes firstChild lastChild firstElementChild lastElementChild nextSibling previousSibling nextElementSibling previousElementSibling nodeType nodeName nodeValue tagName offsetParent  
  - 方法 querySelector() querySelectorAll() appendChild() replaceChild() removeChlid() cloneNode() getAttribute() setAttribute() addEventListener() removeEventListener() 
  - 事件 onclick  ondblclick onmouseenter onmouseleave onmouseover onmouseout onmousemove onmousedown onmouseup onwheel  onkeydown onkeypress onkeyup onscroll transitionend animationend
- 特殊元素对象  input form img video audio canvas
  - img   src  alt  width  height  onload  
  - form  action method enctype name elements  submit() reset() onsubmit onreset 
  - input  type value name disabled readOnly focus() blur() onfocus()  onblur()  onchange() 
  - video audio   play() pause() reload() duration
  - canvas rect() arc() fill()  stroke() filltext() 
- 事件
  - 用户对于网页的一些操作或者浏览器自身的一些行为
  - 事件源 this  事件类型 type  事件处理程序 handler
  - 事件对象 
    - 触发一个事件的时候产生的一个用来记录事件触发详细信息的对象
    - div.onclick=function(e){console.log(e)}
    - div.addEventListener('click',function(e){})
    - $("div").click(function(e){})    
    - 哪些信息 
      - 点击事件  e.clientX e.clientY e.offsetX e.offsetY e.pageX e.pageY
      - 键盘事件  e.keyCode e.ctrlKey e.shiftKey e.altKey
      - e.type  e.target
      - 阻止浏览器默认行为  e.preventDefault() e.returnValue=false
      - 阻止事件流传播  e.stopPropagation()  e.cancelBubble=true
  - 事件流
    - 概念 当我们触发某个元素的事件的时候，它的父元素以及所有的前辈元素一直到页面都会按照特定的方式响应这个事件
    - 划分 冒泡型 捕获型 addEventListener('click',function(){},true)  
    - 阻止    e.stopPropagation()  e.cancelBubble=true
    - 利用    事件委派 * 10000 li 点击  ul  e.target
- cookie
  - http 无状态协议  浏览器 服务器控制在浏览器中生成一条cookie记录 浏览器发送下一次请求的时候 会自动把cookie发送到服务器端 session 凭据
- webstorage
  - localStorage sessionStorage 在浏览器中保存数据 getItem setItem  属性     字符串  JSON.stringify JSON.parse 
- 同源策略 同域   协议+域名+端口号 相同 ajax 跨域 
- reg
  - 工具 使用   //  ^ $ \s \d [a-f1-6] {1,6}  * ? (?:) (?=)
- date
  - api    date.getTime() 获取时间戳 
- ajax
  - ajax 异步JavaScript和XML 
  - 功能：用来完成浏览器和服务器之间的数据交互
  - 特点：在页面不刷新的前提下 对于网页的内容进行局部更新
  - 步骤
    - xhr=new XMLHttpRequest()
    - xhr.open(get,url,async)
    - xhr.send()
    - xhr.onreadystatechange(){
    - xhr.readyState 0 1 2 3 4  xhr.status 200 ok  304 not modified  404 not found  500 server error 
    - }
    - xhr.responseText/xhr.responseXML 
    - xhr.responseType="text" document json ArrayBuffer 
    - xhr.onload   xhr.response
    - xhr.onerror 
    - xhr.onprogress 
    - xhr.ontimeout

# jQuery

- 函数库 

- jQuery和原生JS的区别

  - jQuery是对原生js的封装
  - 解决了一系列的兼容问题
  - 从语法特点  链式调用  隐式循环  查询(获取)功能

- 常用API 方法  html() text() css() addClass() removeClass() toggleClass()  width() height() postion() offset() parent() children() appendTo() append() after() before() insertAfter()  remove() detach() empty() click() mouseenter() 

- ajax 

  - $.ajax()
    - url 请求地址
    - type 请求方式 get post
    - data 发送的数据
    - dataType 接收数据的类型  xhr.responseType  
    - success 成功之后的回调函数
    - async 是否异步
    - processData 是否要转换数据类型 
    - contentType 默认数据类型
    - error 
    - jsonp 当发送的请求是一个jsonp请求的时候  字段名
    - jsonpCallback 字段值 
    - xxx.php?callback=J123123131_13289123781   
  - $.get()
  - $.post()
  - $.getScript()
  - $.getJSON()  

- jsonp 解决跨域请求的一种方式     通过服务器代理请求

  - 和ajax没有直接关系  script标签 jQuery把jsonp封装到$.ajax函数中     
    ​       
    ​    

