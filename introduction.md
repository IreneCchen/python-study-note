## 环境搭建
### anaconda环境配置
> anaconda安装 [官网](https://www.anaconda.com/)  
>> python的一般安装方法：
>>> windows:  
>>> 1、 https://www.python.org/downloads/ 选择适合自己电脑的最新版本 （30M）  
>>> 2、配置环境变量   
>>>【右键计算机】--》【属性】--》【高级系统设置】--》【高级】--》【环境变量】--》【在第二个内容框中找到 变量名为Path 的一行，双击】 --> 【Python安装目录追加到变值值中，用 ； 分割】  
>>> 如：原来的值;C:\python37，切记前面有分号  
>> mac、linux自带。

 ***
### 安装配置指南
anaconda个人理解： anaconda像是python的一个集成环境，以数据科学为主，包含python的多种解释器，可以构建独立构建不同的python依赖环境，具有很高的扩展性。如果说python是胶水语言的话，anaconda就是装胶水的瓶子，能将胶水应用于数据科学，web应用，人工智能，程序设计等各种领域。
### 解释器  
Python是解释型语言（面向对象）  
#### Python的解释器分类：
* CPython（官方） 用c语言编写的Python解释器
* PyPy 用Python语言编写的Python解释器
* IronPython 用.net编写的Python解释器
* Jython 用Java编写的Python解释器

***
## python是一门动态解释性的强类型定义语言。
### python的优缺点
> 优点  
>> 1、Python的定位是“优雅”、“明确”、“简单”，所以Python程序看上去总是简单易懂，初学者学Python，不但入门容易，而且将来深入下去，可以编写那些非常非常复杂的程序。  
>> 2、开发效率非常高，Python有非常强大的第三方库，基本上你想通过计算机实现任何功能，Python官方库里都有相应的模块进行支持，直接下载调用后，在基础库的基础上再进行开发，大大降低开发周期，避免重复造轮子。  
>> 3、高级语言————当你用Python语言编写程序的时候，你无需考虑诸如如何管理你的程序使用的内存一类的底层细节  
>> 4、可移植性————由于它的开源本质，Python已经被移植在许多平台上（经过改动使它能够工 作在不同平台上）。如果你小心地避免使用依赖于系统的特性，那么你的所有Python程序无需修改就几乎可以在市场上所有的系统平台上运行  
>> 5、可扩展性————如果你需要你的一段关键代码运行得更快或者希望某些算法不公开，你可以把你的部分程序用C或C++编写，然后在你的Python程序中使用它们。  
>> 6、可嵌入性————你可以把Python嵌入你的C/C++程序，从而向你的程序用户提供脚本功能。 

> 缺点  
>> 1、速度慢，Python 的运行速度相比C语言确实慢很多，跟JAVA相比也要慢一些，因此这也是很多所谓的大牛不屑于使用Python的主要原因，但其实这里所指的运行速度慢在大多数情况下用户是无法直接感知到的，必须借助测试工具才能体现出来，比如你用C运一个程序花了0.01s,用Python是0.1s,这样C语言直接比Python快了10倍,算是非常夸张了，但是你是无法直接通过肉眼感知的，因为一个正常人所能感知的时间最小单位是0.15-0.4s左右，哈哈。其实在大多数情况下Python已经完全可以满足你对程序速度的要求，除非你要写对速度要求极高的搜索引擎等，这种情况下，当然还是建议你用C去实现的。    
>> 2、代码不能加密，因为PYTHON是解释性语言，它的源码都是以名文形式存放的，不过我不认为这算是一个缺点，如果你的项目要求源代码必须是加密的，那你一开始就不应该用Python来去实现。    
>> 3、线程不能利用多CPU问题，这是Python被人诟病最多的一个缺点，GIL即全局解释器锁（Global Interpreter Lock），是计算机程序设计语言解释器用于同步线程的工具，使得任何时刻仅有一个线程在执行，Python的线程是操作系统的原生线程。在Linux上为pthread，在Windows上为Win thread，完全由操作系统调度线程的执行。一个python解释器进程内有一条主线程，以及多条用户程序的执行线程。即使在多核CPU平台上，由于GIL的存在，所以禁止多线程的并行执行。关于这个问题的折衷解决方法，我们在以后线程和进程章节里再进行详细探讨。  

***
## 变量、赋值、数据
### 变量  
> 用于存储要在计算机程序中引用和操作的信息。它们还提供了一种用描述性名称标记数据的方法，以便读者和我们自己能够更清楚地理解我们的程序。将变量看作包含信息的容器是有帮助的。它们的唯一目的是在内存中标记和存储数据。然后可以在整个程序中使用这些数据。
#### 变量定义的规则：
* 变量名只能是 字母、数字或下划线的任意组合
* 变量名的第一个字符不能是数字
* 以下关键字不能声明为变量名
['and', 'as', 'assert', 'break', 'class', 'continue', 'def', 'del', 'elif', 'else', 'except', 'exec', 'finally', 'for', 'from', 'global', 'if', 'import', 'in', 'is', 'lambda','not', 'or', 'pass', 'print', 'raise', 'return', 'try', 'while', 'with', 'yield']
### 变量的赋值：  
name = "Zhichao"  
name2 = name  
print(name,name2)  
name = "Han-Teng"  
print("What is the value of name2 now?")  
