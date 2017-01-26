# Chapter 2  函数

`[[Call]]`属性是函数独有的，表示本对象可以被执行。由于仅函数拥有该属性，ES把`typeof`操作符对任何具有`[[Call]]`属性的对象返回`fuction`

本章讨论在JavaScript中定义和执行函数的各种方法。由于函数是对象，它们的行为和其他语言中的函数行为也不同，因此理解函数的行为是理解JavaScript的核心。


### 2.1 声明or表达式？

- 函数声明
```
function add(num1 , num2){
    return num1 + num2;
}
```
- 函数表达式
```
function add(num1 , num2){
    return num1 + num2;
}
```


### 2.2 函数就是值

### 2.3 参数

### 2.4 重载

### 2.5 对象办法

2.5.1 `this`对象

2.5.2 改变`this`

### 2.6 总结