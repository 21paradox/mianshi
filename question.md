#面试题搜集

##javascript

###Numbers

```javascript
    a = 0.1; 
    b = 0.2; 
    c = 0.3;
    
    (a + b) + c === a + (b + c) //false 为什么错了？
 
```

请写出下面运算式的结果

```javascript
    5 / 5
    5 /  "5"
    5 / "5a"
    5 / "NaN"

```

```javascript
parseInt("08") === 0 // ie 8

如何处理这种情况

```


### Array

如何删除数组中的第二项 

```javascript
   var arr = ['a','b','c','d'];
   
   arr ==> ['a','c', 'd']
   
 
   
```

如何检测 一个对象是不是数组呢
```javascript
    var arr = ['a','b']
提示：
    typeof arr === 'object',
    typeof null === 'object'
    
 
```


### Boolean
写出下面的运算结果
!!会把一个对象变成布尔值
```javascript
    !!false
    !!null 
    !!undefined 
    !!"" 
    !!0
    !!NaN
 
    !!"0"  
    !!"false" 
    !!{} 
 
 
    function myfunc(config){
        if(config){
            ...
        }
    }
    
```

arguments 对象

```javascript
    //解释一下 arguments 对象 （存在于function中的）
 arguments对象和数据

```



prorotype原形继承 
```javascript

var Vm= function(id){
    this. id = id;
}
Vm.prototype.getGame = function(){
    return $.ajax ...
}

写出一个继承 vm的例子

```
 
预热题不计入考察

```javascript
function funky(o){ 
    o = null; 
}

var a = []; 

funky(a);

 // a是多少？

```

```javascript
function swap(a,b){
    var temp = a;
    a = b; 
    b = temp; 
}
var x =1, y = 2;

swap(x,y)

// x多少， y多少
 
```

请写出一个函数 可以这样执行：calc(3)(2) //计算结果是5
 <br><br>

请写出一个函数 可以这样执行：assertPlus(3,2)(5) //(如果 3+2 === 5 ,返回 true,否则返回 false)
 <br><br>
 
### jQuery相关

如何用jQuery检测这个dom是否存在页面
<br><br>

jQuery检测页面的元素是否可见？
<br><br>

jQuery删除页面的元素和绑定事件
<br><br>

jQuery请求2个接口，并且在2个接口返回之后 执行console.log
   提示:可以用$.when
<br><br>

上述问题如果用es6的Promise封装之后应该怎么写？
<br><br>

json的key和value可以用单引号吗？
<br><br>

es6的let 定义变量和var的 区别
<br><br>


##npm

如何安装nodejs，linux服务器没有root权限如何安装？
<br><br>

如何安装项目所有依赖？
<br><br>

npm 项目中如何执行自定义脚本
<br><br>

如何升级项目依赖的库？
<br><br>

有使用过browserify吗，它有什么优点缺点？
<br><br>

##css

inline 和 block的区别
```css
分别用inline 和 block 实现居中效果

float left 使元素从左向右排列
float right 使元素从有向左排列

如何清除浮动


写一个水平垂直居中的css样式


bootstrap 3 使用了box-sizing: border-box ，解释一下 border-box 和context-box区别
```

##svg

svg坐标和html的区别
<br><br>

svg的viewPort有什么特点，一般会在哪里使用到
<br><br>

svg的 <g>如何布局，和div布局的区别
<br><br>

angular/react中使用svg需要注意的，写一个svg时钟demo
<br><br>








 
 
