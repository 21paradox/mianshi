##面试题搜集

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
   
   delete arr[1] // 为什么这样用是错误的
   
   arr.splice(1,1) //正确方法
   
```

如何检测 一个对象是不是数组呢
```javascript
    var arr = ['a','b']

    typeof arr === 'object',
    typeof null === 'object'
    
    $.type(arr)   //jQuery
    Array.isArray(arr)    //es5
    Object.prototype.toString.call(arr) === '[object Array]';   //es3

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
    //上面的都是 false
    
    !!"0" //true
    !!"false" //true
    !!{} //true
    
    //实际使用情况
    
    
    function myfunc(config){
        if(config){
            ...
        }
    }
    
```

arguments 对象

```javascript
    //解释一下 arguments 对象 （存在于function中的）
    //是一个 类似 数组的对象, 没有slice splice 等方法
    
    arguments.length    //有length属性

```

调用function的四种形式

```javascript
    func() //直接调用
    new func() //实例化
    myfunc.func() //类似方法的调用
    func.apply(this,'1') //用 apply或者 call指定 this调用
```

###闭包

IIFE
```javascript
    //IIFE = Immediately-Invoked Function Expression.
    //写一个 IIFE
    
    // good
    var task = (function () {
       // Code
       return result;
    })();
    
    
    var task = (function(){
        //Code
        return result;
    }())
    
    //上面两种都是可以的
```


```javascript
    //一个闭包的例子
    
    define(function(require,exports,module){
        
        var token = '12345';
    
        module.exports = {
            checkToken: function(tkNew){
                return tkNew === token;
            }
        }
    
    })  //定义一个私有变量token,检测 token是否合法，seajs

```


#### 这些还未完成
prototype

module pattern

private variable

function hoisting



预热题不计入考察

```javascript
function funky(o){ 
    o = null; 
}

var a = []; 

funky(a);

//运行之后 a === []

```

```javascript
function swap(a,b){
    var temp = a;
    a = b; 
    b = temp; 
}
var x =1, y = 2;

swap(x,y)

//运行之后 x === 1, y ===2
```

请写出一个函数 可以这样执行：calc(3)(2) //计算结果是5

```javascript
 var calc = function (a){
    return function(b){
        return a + b;
    }
 }

```


请写出一个函数 可以这样执行：assertPlus(3,2)(5) //(如果 3+2 === 5 ,返回 true,否则返回 false)
```javascript
function assertPlus(a ,b){
		return function(c){
			return  c === a + b;
		}
	}
```




####这些还未完成

jquery $.map $.extend $.ajax

$.when $().end

check if dom exists

json

 
 
