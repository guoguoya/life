﻿# 问题

1. 在响应式布局中，属性类的局限性。（2017.2.6）
描述
当大量使用(pll, prl, mlm, fz-md) 这种抽象的内容在用px的时候并不能很好的支持响应式布局 。 
解决方式

在局部小区域内可以用 

2. 如果我将组件的js 和less 写在一起， 在写库的时候没有问题 ，我可以认为各个库里的组件是相互不影响的，


3.class 上的fn默认在babel编译时是不能遍历的，在chrome 上 class 上的fn 默认也是不能遍历

那么如何获取class 上的所有fn ？
解决方法

getPrototypeOf 

通过 Object.getOwnPropertyNames 获取所有自身属性

维护一个key对象，过滤掉一些不必要的属性 


4.当调用一个未声明时js编译器会报错， 比如 a ;
但是当 存在运算 比如a = 1; 这是默认声明并赋值 a。
那么如何判断一个 变量是否申明 用typeof ，未申明的变量是 'undefined'。