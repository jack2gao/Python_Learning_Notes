# 前置学习
## 1.Pycharm的安装
### pycharm的安装环境

### pycharm的环境配置
### pycharm的基础使用

## 2. vim的基础使用
安装 idea vim插件
## 3. markdown的基础使用
[Markdown](https://www.runoob.com/markdown/md-advance.html)
## 4. git的基础使用
**可以后续在做增加学习**


# 0305学习笔记

## 学习规则说明
###内部系统的使用机制
* 课程的时间安排,周末及平时  
* 周末全天课程(10:00-16:00)，平时晚上课(19:00-21:30)  
* 课程日历课程排期
* 作业提交
* 积分规则 加分+交作业+质量好+看视频  
**每日任务:** 每天交一份作业，每天看两个视频  
**扣分:** 隔72小时检查一次
```看视频在哪里？？```

_作业先看了别人的作业，在上传，不算今天的当日任务_

PK机制促进大家的学习  
勋章强，点亮所有

### 整体课程
* Python基础，基础知识的掌握  
* 网络经典协议实现自动化，替代人工操作，自动批量实现  
* Django的自动化，从代码替代命令行解决问题，到通过工具平台标准化和自我实现  
* DevNet目前的网络都已经实现了API的方式对设备操作，对工作也是最直接的支持    
* 开源的软件系统是成熟的专业的沉淀，能够支撑未来业务的快速成熟  
* 自动化运维系统开发实例，做一个实践练习。  

```DevOps/DevSecOps为社么要区分```

### Python基础
基础课应该是最重要的，入门的过程也是最难的，更需要比较系统和全面的认知。
后面可能比较使用，但如果走的远，则需要扎实基础。

四大模块
1. 基础字符
2. 字符类型
3. 类模块
4. 高阶部分

### 语言的现状；
Python很火
Python基于灵活优势在自动化运维等方面非常流行，当然也会有数据分析/人工智能/
大型系统平台的主要还是C，Java等，
比如语音开发K8S，云原生开发，则是选择GO
网页前端，JavaScript极具优势

首先基于网络的专业基础，叠加自动化的工具，
网络很难,Python不难，所以基于专业叠加技能会更适合

```为什么说Python适合所有人？
因为简单，学习坡度低，开发效率高，叠加技能能够实现效率的指数级提升，以及自动化成为可能
```
##  Python应用领域
云计算，AWS,GO  
大型网站，效率，可靠性不够，主要体现在架构的配合等方面，  
Python开发效率高，最小原型是一个适用场景，  
人工智能/大数据，基础数学等必须要有非常深的研究。Python的工具提效和实现。    
自动化运维，前提是对业务（事）非常熟悉和理解，然后通过自动化实现。  
**需要基础的知识加实践练习，可以达成**
大数据的应用也是，基于对量化交易等熟悉。
网页呈现更多,BS架构


## Python哲学
就是解决问题
就是简单的一种道路
否定高级感，复杂实现

体会下Python和其他语言的差异，以及他成功的关键

* 优雅
简洁干练，没有多余的语法结构
* 明确
强制要求格式统一，缩进，代码块层级

### 超高级语言
* 脚本 高级语言  胶水语言  
直接解释器运行，无需编译过程
接近人的认知，但性能差，不做加密
Pthon调用核心库，配合C实现提效。
通过对逻辑的连接模块调用，实现一个业务的结果，而这些核心的模块往往通过C/JAVA等专业语言。

>目标：  
>开发速度?  
>运行速度？

发生频率并不高，时效性并不重要的场景

避免出错，提升效率

* 功能强大适用方便

强大的社区生态，内置标准库，丰富强大的三方库

1. 可移植性
通过解释器评估了系统差异
2. 


---上午10:00-12:00--
## Python安装

[Python](https://www.python.org/downloads/)

Window：
选择正式版本3.8即可，注意安装的目录增加到Path勾选，下一步直接操作  
>目的：
> 第三方模块对于最新的适配可能还存在问题

Linux:
当前Linux主流主要Centos7,还是Python2.0，可以参考手册增加Python3.X，多个版本共存
学习为目的，安装过程建议关闭防火墙
>systemctl status firewalled
> SELINUX = disable
> 

## pip模块安装

pip install _[module]_ -i _[国内服务器]_

>stream??  
kamene
requests
netmiko


必须支持：
Linux  
DB(mysql)
正则表达

建议Pycharm编辑器

文档搜索建议:google


## Python的类型

### Python内置对象
* 内置对象让程序书写更方便
* 标准
* 高效

不可变类型：  

Numbers
Strings

可变类型   
Lists
Dictionaries
Turples
Files
Sets

--Numeric
--Sequence
--Mapping
--Sets

#### 基本数字常量 Numbers
--整数
--小数
--复数

数字操作
Expression Operator 表达式操作    
-- +  - * / >> <<  
Built-in mathematical function 内建数学函数  
-- abs() pow()  
Utility modules（工具模块）
-- sum(),min(),max(),sorted()


#### random
```
import random

random.random() 
//0,1之间的随机数
random.randomint()

rand
```


### 字符串内置类型

* 序列 不可变类型  

单引号  
双引号  
三引号  ：
多端字符串的描述

>引号之间如果增加引号，则通过\”来进行转义
\n 换行
\t 制表符
\r 回车  

如果对于有特殊字符的字符串要进行字符输出
1. 通过转义符来进行输出
print("c:\\programfile\\user\\pyton.txt")
2. 通过Raw strings即前面加r
print(r"c:\programfile\user\python.txt")

b字节字符串
Bytes literals in 3.x/2.6x
b'sp\x01am'
**ASCII字符会本自动转码
print(b'\x73\x70\x01\x61\x6d')
```字节字符串
>>> print(b'\x73\x70\x01\x61\x6d')
spam
```

*python有每行的长度建议，通过\来进行换行输出*

>window文本每一行最后\n\r  
> Linux文本每一行最后\n  
> MAC系统文本每行最后\r  

字符串可以通过 + 号进行字符串的拼接
> string = "hello" + " world!"
> print(string)

字符串可以通过* 和数字组合进行相乘
> stringNumber = "hello world!" * 2
> print(stringNumber)

因为是字符串有序列的特点可以进行循环输出，或者进行字符包含关系的判断
```字符串的循环读取操作实例
string = 'heaker'
for i in string:
    print(i,end='')
```
可以通过条件设定进行判断
```字符串的包含关系
string = 'heaker'
if "er" in string:
    print(" er in " + string)
```

以为有序列关系可以进行顺序操作
```切片操作
>>> s = "hello world!"
>>> s[10]
'd'
>>> s[1:10]
'ello worl'
>>> s[1:]
'ello world!'
>>> s[1:-2]
'ello worl'
```

```不可变类型不能修改
>>> s[1]
'e'
>>> s[1]='u'
Traceback (most recent call last):
  File "<stdin>", line 1, in <module>
TypeError: 'str' object does not support item assignment
>>>
```

#### 字符串对象的方法
对象是一个类的实例，他拥有该类的所有方法采用
这个只会返回一个新的结果，可以用一个变量收集这个修改，原来的对象不变
> string.lower()  
> string.upper()
> "!".join(string)

函数是通过对数据变量的操作返回结果，有内置函数可以实现特定该功能
> len(string)
> type(string)


字符串的格式化表达式
目的是对数据进行格式化，既能够实现良好交付，也是能够结构化额处理

1. 格式

2. 字符串格式化的方法 string.formate()

3. f方法

### 正则表达式

将设备返回的字符串结构化，然后进行数据处理
cisco：  
* pyats  
* ntc-template

通用的做法一般通过正则进行匹配和处理。

正则在网络中：
BGP的as-path匹配
show | reg 的匹配

特殊字符需要进行转译\


#### 匹配次数
{n}     重复N次  
{m,n}   至少重复m次，最多出现n次  
{m,}    至少重复m次  
?       {0,1}  
\+      {1,}  
\*      {0,}

匹配IP地址
([0-2]?[0-5]?[0-5]?\.){3}([0-2]?[0-5]?[0-5]?)
#### 起始终止位置
```
^
$
\b
```

#### 抽象代表


查找数据
```Python

string1 = "hello"
string2 = "world!"
string3 = "python"
number1 = 100.12345

string = "%s  %-10s"

# -左对齐
# 6 宽度
#.小数点后2位置
#f浮点数

#+左补零，在%右侧属于占位


string4 = "{}.{} and {}".format(string1,string2,string3)
string5 = "{0:>10}={1:<10} = {2:^10}".format(string1,string2,string3)
print(string4)
print(string5)

string6 = f'{string1:^10} ={string2:<10}'
print(string6)


import  re

re_1 = "cmd.exeabcde"
re1 = re.match("cmd\.exe",re_1)
print(re1)
re2 = re.match(".*","cmd.exe\n\s\tceshi.exe")
print(re2)
re3 = re.match("[\s\S]*","cmd.exe\n\s\tceshi.exe")
print(re3)

#ip_regx = "([0-2]?[0-5]?)"
#ip_regx = "([0-2]?[0-9]?[0-9]?\.){3}([0-2]?[0-9]?[0-9]?)"
ip_regx = "([0-2]?[0-9]?[0-9]?)\.([0-2]?[0-9]?[0-9]?)\.([0-2]?[0-9]?[0-9]?)\.([0-2]?[0-9]?[0-9]?)"
ip = "192.168.1.1"
r4 = re.match(ip_regx,ip)
print(r4)
groups_ = r4.groups()
print(groups_)
```
替换数据
```Python
import re
string5 = re.sub("[=-]+","--","aaaa===bbb--ccc=aa=")
print(string5)

```


