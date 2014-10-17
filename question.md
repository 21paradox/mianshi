#面试题搜集

##javascript

###Numbers

```javascript
    a = 0.1; 
    b = 0.2; 
    c = 0.3;
    
    (a + b) + c === a + (b + c) //false 
 
```

请说出下面运算式的结果

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

删除数组中的第二项 

```javascript
   var arr = ['a','b','c','d'];
   
   arr ==> ['a','c', 'd']
   
 
   
```

如何检测 一个对象是不是数组呢
```javascript
    var arr = ['a','b']

    typeof arr === 'object',
    typeof null === 'object'
    
 
```


### Boolean

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
 

```

调用function的四种形式

```javascript
    func() //直接调用
    ..
	..
	..
```

###闭包

IIFE
```javascript
    //IIFE = Immediately-Invoked Function Expression.
    //写一个 IIFE
    
 
 
```


```javascript
    //一个闭包的例子
    
 

```


prorotype原形继承 
```javascript



var Vm= function(id){
    this. id = id;
}
Vm.prototype.getGame = function(){
    return $.ajax ...
}

 

```
 
预热题不计入考察

```javascript
function funky(o){ 
    o = null; 
}

var a = []; 

funky(a);

 

```

```javascript
function swap(a,b){
    var temp = a;
    a = b; 
    b = temp; 
}
var x =1, y = 2;

swap(x,y)

 
```

请写出一个函数 可以这样执行：calc(3)(2) //计算结果是5
 

请写出一个函数 可以这样执行：assertPlus(3,2)(5) //(如果 3+2 === 5 ,返回 true,否则返回 false)
 
 

jquery $.map $.extend $.ajax

$.when $().end

check if dom exists

json

 
 
##css


inline 和 block的区别
```css
//分别用inline 和 block 实现居中效果
 

//float left 使元素从左向右排列
//float right 使元素从有向左排列

如何清除浮动

 
会制作雪碧图吗 css sprite
photoshop 选中图层，复制图层



```

 
 
