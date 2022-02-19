# 1.基础部分 

**1.1  JDK和JRE的区别是什么？**

Java运行时环境(JRE)是将要执行Java程序的Java虚拟机。它同时也包含了执行applet需要的浏览器插件。

Java开发工具包(JDK)是完整的Java软件开发包，包含了JRE，编译器和其他的工具(比如：JavaDoc，Java调试器)，可以让开发者开发、编译、执行Java应用程序。

**1.2  Java基本的八大数据类型**

int 、float  、double、byte、short、long、char、boolean

**1.3  String的特点**

String 是 final修饰的类，不能被继承，并且他的成员方法也默认都被final修饰。  实际上是通过char[] 数组的来保存字符串的。 每次函数操作都是生成了新的String对象，

**1.4 包装类型  int 和 Integer**

int是基本数据类型，Integer是引用对象类型，一个默认值为0，一个默认为null。 Integer在-128-187之间的整数会有缓存，在赋值的时候直接取，不会开辟空间去new。

**1.5  switch支持的数据类型**

在JDK1.5之前,switch循环只支持byte short char int四种数据类型.

JDK1.5 在switch循环中增加了枚举类与byte short char int的包装类------》对四个包装类的支持是因为java编译器在底层手动进行拆箱,而对枚举类的支持是因为枚举类有一个ordinal方法,该方法实际上是一个int类型的数值.

JDK1.7在switch循环中增加了String类型-------》但实际上String类型有一个hashCode算法,结果也是int类型.

**1.6  方法的重载和继承**

重载：方法名相同、参数不同    继承：继承、覆盖的方法。

**1.7  面向对象的特点**

封装：

继承：

多态：

**1.8 static修饰符和特点**

类中可以有多个static块。在类初次被加载的时候，会按照static块的顺序来执行每个static块，并且只会执行一次。 静态方法  静态成员。

**1.9 StringBuilder和StringBuffer**

都是final类，不允许被继承，StringBuffer是线程安全的。

**1.10  异常Error和Exception**

一个是错误，一个是异常。

**1.11  线程 并行和并发  进程和线程之间的概念**

并发：一个处理器可以同时处理多个任务。这是逻辑上的同时发生。
并行：多个处理器同时处理多个不同的任务。这是物理上的同时发生。
有一个清晰地比喻：
并发：一个人同时吃三个苹果。并行：三个人同时吃三个苹果。

单位不同， 一个进程可以有很多个线程。

![image-20220218183805718](C:\Users\lww\Desktop\aa\javaNotes\java基础知识.assets\image-20220218183805718.png)

**1.12 线程启动的几种方式**

**1.13  线程不安全相关问题以及锁  day14  11-17**

**1.14 线程通信相关**

**1.15  ArrayLIst、LinkedList、栈、哈希表（HashTable） 相关优缺点以及特征**

**1.16 集合框架**

**1.17  IO流 输入输入流、缓冲流 等等。**

**1.18  NIO概述 day21 - 12**

**1.19 反射**

**1.20 JAVA8新特性**

