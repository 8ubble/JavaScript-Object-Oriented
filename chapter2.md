# Chapter 2  函数

`[[Call]]`属性是函数独有的，表示本对象可以被执行。由于仅函数拥有该属性，ES把`typeof`操作符对任何具有`[[Call]]`属性的对象返回`fuction`

本章讨论在JavaScript中定义和执行函数的各种方法。由于函数是对象，它们的行为和其他语言中的函数行为也不同，因此理解函数的行为是理解JavaScript的核心。


### 2.1 声明or表达式？

- 函数声明：`function`关键字+函数名
```
function add(num1 , num2){
    return num1 + num2;
}
```
- 函数表达式：`function`后面不需要加函数名
```
var add = function(num1 , num2){
    return num1 + num2;
};
```
- 可以先使用函数再进行声明。

### 2.2 函数就是值
只要是可以使用其他引用值的地方，就可以使用函数。
```
function sayHi(){
    console.log("Hi!"); //outputs "Hi!"
}
sayHi();

var sayHi2 = sayHi;

sayHi2();               //outputs "Hi!"
```
和下面这段代码的功能是一样的：
```
var sayHi = new Function("console.log(\"Hi!\");");
sayHi();               //outputs "Hi!"
var sayHi2 = sayHi;
sayHi2();
```

**记得：`函数就是对象`**
### 2.3 参数
JavaScript函数的另一个独特之处在于你可以给函数传递任意数量的参数却不造成任何`bug`（因为函数参数实际上被保存在一个`arguments`的类似数组的对象中）。

函数的命名参数不过是为了方便，并不真的限制了该函数的可接受参数的个数。

P.S. `arguments`对象不是一个数组的实例，其拥有的方法与数组不同，`Array.isArray(arguments)`永远都返回`false`

### 2.4 重载

### 2.5 对象办法

2.5.1 `this`对象

2.5.2 改变`this`

### 2.6 总结