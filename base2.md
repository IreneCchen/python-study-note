### if...else
Python 条件语句是通过一条或多条语句的执行结果（True 或者 False）来决定执行的代码块。  

可以通过下图来简单了解条件语句的执行过程:  
![](if-condition.jpg)
代码执行过程：
![](python-if.webp)
* if 语句  
Python中if语句的一般形式如下所示：  
if condition_1:  
    statement_block_1  
elif condition_2:  
    statement_block_2  
else:  
    statement_block_3  
如果 "condition_1" 为 True 将执行 "statement_block_1" 块语句  
如果 "condition_1" 为False，将判断 "condition_2"  
如果"condition_2" 为 True 将执行 "statement_block_2" 块语句  
如果 "condition_2" 为False，将执行"statement_block_3"块语句  
Python 中用 elif 代替了 else if，所以if语句的关键字为：if – elif – else。  

* 注意：  
1、每个条件后面要使用冒号 :，表示接下来是满足条件后要执行的语句块。  
2、使用缩进来划分语句块，相同缩进数的语句在一起组成一个语句块。  
3、在Python中没有switch – case语句。  
* if 嵌套  
在嵌套 if 语句中，可以把 if...elif...else 结构放在另外一个 if...elif...else 结构中。  

### 迭代
* 如果给定一个list或tuple，我们可以通过for循环来遍历这个list或tuple，这种遍历我们称为迭代（Iteration）
* Python的for循环不仅可以用在list或tuple上，还可以作用在其他可迭代对象上。list这种数据类型虽然有下标，但很多其他数据类型是没有下标的，但是，只要是可迭代对象，无论有无下标，都可以迭代

>for循环/range

* For … in 语句是另一种循环语句，其特点是会在一系列对象上进行迭代（Iterates），即它会遍历序列中的每一个项目
注意：

1、else 部分是可选的。当循环中包含它时，它循环中包含它时，它总会在 for 循环结束后开始执行，除非程序遇到了 break 语句。

2、for … in 能在任何队列中工作。有的是通过内置 range 函数生成一串数字列表，也可以是包含任何类型对象的队列。

* range（）函数
一般形式：range（start，stop[，step]） 

start ：开始数值，数值为0，也就是如果不写这项，则认为start = 0 。  
stop ：结束的数值，这是必须要写 。  
step ：变化的步长，默认是1 。

### random函数
1、random() 方法返回随机生成的一个实数，它在[0,1)范围内。  
2、random()是不能直接访问的，需要导入 random 模块，然后通过 random 静态对象调用该方法。  
