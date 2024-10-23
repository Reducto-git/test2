# Java02-程序基本结构-程序基本结构

## **Task1.单文件代码结构**

### （1）

#### 1.1解释每个部分

```java
package com.ISEKAI;
```
**包声明**：包是Java中的一种命名空间，帮助开发者将相关的类和接口分组，使得代码更易于管理和维护。同时，包也控制了类的可见性，只有同一包中的类可以直接访问包内的类，否则需要`import`。

```java
import com.ISEKAI.tool.Print;
```
**导入语句**：用于导入其他包中的类。这里引入了`com.ISEKAI.tool`包中的`Print`类。

```java
public class HelloWorld {
    public static void main(String[] args){
        Test.test();
    }
}
```
**主类**：`main`函数是Java程序的入口点，是程序执行的起始位置。JVM（Java虚拟机）从这里开始执行程序。

```java
class Test {
    public static void test(){
        Print.print("Hello World");
    }
}
```
**辅助类**：这是一个自定义的辅助类`Test`，包含一个静态方法`test`，它负责调用`Print`类中的`print`方法。

#### 1.2单文件Java程序的基本结构

* 包声明

* 导入其他类
* 主类
* 辅助类

### （2）

#### 2.1修改main函数

```java
public static void main(String[] args){
    for (String arg : args) {
        System.out.println(arg); 
    }
}
```

#### 2.2运行程序

见附件“改造main传入参数.mp4”

## **Task2.多文件Java项目**

### （3）

```java
package com.ISEKAI.tool;

public class Print {
    public static void print(String message) {
        System.out.println(message);
    }
}
```

运行截图见“打印HelloWord.pong”

