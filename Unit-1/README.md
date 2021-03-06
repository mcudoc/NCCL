﻿NCCL - New Concept C Language
=============================

### 《新概念C语言》Unit 1 视频学习课件
* 全套42集免费视频课程已经发布，通过百度云盘可以下载，也可以在线观看视频（手机安装百度云也可以在线观看）。
	- 视频下载地址 <http://pan.baidu.com/s/1jGjxusA>
	- 视频中所有用到的范例C程序[代码下载](https://github.com/limingth/NCCL.codes)
	
* 推荐使用播布客网站视频播放器本地观看视频，更清晰更流畅。 <http://www.boobooke.com/video.html>
	- 播布客[视频播放器下载](http://www.boobooke.com/download/MBoo2014.zip)
	
* 《新概念C语言课程概述》(第0集) 在线观看 <http://www.boobooke.com/v/bbk5910/>

* 《C程序设计语言（第2版-新版）》多贝网络公开课在线观看 <http://www.duobei.com/course/5334465437>
	- 参考用书《K&R》[下载链接](https://www.dropbox.com/s/qer3va6rtq8o1dj/C%E7%A8%8B%E5%BA%8F%E8%AE%BE%E8%AE%A1%E8%AF%AD%E8%A8%80%EF%BC%88%E7%AC%AC2%E7%89%88%C2%B7%E6%96%B0%E7%89%88%EF%BC%89.pdf)

### 一对一远程视频辅导
* 新概念C语言 Unit 1 和 [Unit 2](../Unit-2/README.md) 开始提供一对一编程辅导课程，学习时间2-3个月。
	- 个性化辅导，根据个人接受程度，灵活安排上课时间
	- 报名学习请咨询 QQ: 2372614758 （亚嵌李明老师）

* 提前安装学习环境
	- [下载安装 Google Chrome 浏览器](http://www.google.com/intl/zh-CN/chrome/)
	- [注册 Gmail 帐号](https://accounts.google.com/SignUp?service=mail&continue=https%3A%2F%2Fmail.google.com%2Fmail%2F&ltmpl=default&hl=zh-CN)
	- [美国地区的学员请安装 Google Hangout 环聊](https://www.google.com/tools/dlpage/hangoutplugin?)
	- [国内地区不能翻墙的学员请下载注册 Skype 帐号](http://www.skype.com/zh-Hans/download-skype/skype-for-computer/)


### 开发环境选择
* 推荐安装 Ubuntu Linux，并安装以下包
	- sudo apt-get install manpages-dev gcc make libc6-dev

* 对于从来没有安装过 Ubuntu（包括虚拟机） 的初学者，最好的选择是
	- 直接通过 [nitrous.io](http://www.nitrous.io) 网站来学习 Linux C 编程
	- 好处就是可以通过浏览器来获得 Linux 编程环境，无需安装Ubuntu操作系统，节省时间
	- 更有用的是只要能够上网的地方，就能获得C编程的环境，无需带虚拟机或双操作系统到处跑

* 如果希望能够在 Windows 上使用 Gcc 开发工具，可以安装 MinGW，参考安装流程
	- http://blog.csdn.net/firefoxbug/article/details/6724876

* 如果需要安装 VC6.0 ，可以到这里下载 <http://see.xidian.edu.cn/cpp/html/1117.html>

* nitrous 浏览器登录界面如下

![nitrous.io](../images/nitrous.jpg)

### Mac 苹果笔记本环境安装
* Mac 上运行播布客软件，可以采用 WINE 的解决方案。
	- <http://linfan.info/blog/2012/03/01/wine-mac/>

* 具体步骤如下
	- 到 [http://brew.sh](http://brew.sh) 下载安装 brew ，也可以直接运行下面的命令
	- ruby -e "$(curl -fsSL https://raw.github.com/Homebrew/homebrew/go/install)"
	- brew doctor 将检查到的 warning 问题排除
	- brew install wine --devel
	- https://xquartz.macosforge.org/landing/  下载 XQuartz-2.7.5.dmg 并安装Mac OS下的 X Window System 
	- http://linfan.info/blog/2012/02/25/homebrew-installation-and-usage/


# Unit One
Unit 1 是《新概念C语言》系列课程的第一部分，共有24个Lesson，包含以下4个层次的学习内容：

1. Beginning Lessons (Lesson 1-7)  
    以变量为核心，运用循环语句和条件分支，讲解C程序的基本结构。

2. Intermediate Lessons (Lesson 8-14)  
    以数组为核心，分析常用数据结构(字符串，结构体，联合)，讲解C程序的函数设计。
  
3. Advanced Lessons (Lesson 15-21)  
    以指针为核心，结合二维数组，位操作和函数指针，讲解C程序的状态机编程思想。

4. Homework Projects (Lesson 22-24)  
    以任务为核心，通过趣味题，综合使用学习过的知识和技能，实现项目需求功能。

# Beginning Lessons

## Lesson 1 [What is the simplest C program?](Lesson-1.md) 最简单的C程序
* C 语言 Language
	- 高级语言 High-level Programming Language
	- 汇编语言 Assembly Language
	- 机器指令 Instructions
* 编译器 Compiler
	- 汇编器 Assembler	
* 操作系统 OS
	- 加载器 Loader
	- 加载地址和执行地址 Load_Addr & Exec_Addr	
* 程序的执行 Program Execution
	- 进程的概念 Process 
	- 执行流程 Execution Sequence

## Lesson 2 [Let's say hello to world](Lesson-2.md) 打印输出
* 库函数 Library
	- libc & glibc
	- 系统调用 System Call
	- 库封装了系统调用
* 链接器 Linker
	- 链接脚本 Link Script
	- 程序入口 Entry
	- 链接脚本决定了程序的执行地址 
* 程序的编译过程 Program compiling procedure
	- 预处理 Preprocessing  cpp (.c -> .i)		
	- 编译 Compilation  cc1 (.i -> .s)
	- 汇编 Assembly  as (.s -> .o)
	- 链接 Linking  collect2 (.o -> .elf)
* 虚拟地址 Vitual Memory Address
	- 进程独立的地址空间 
	- 内存管理单元 MMU 

## Lesson 3 [Count how many fingers do you have?](Lesson-3.md) 循环打印
* while 循环 和 do-while 用法
	- 比较和跳转指令 Compare and Jump Instruction
	- do-while 比 while 有时更有用
* 变量的初始化 Variable Initialization
	- 变量的存储布局 Data & BSS Section
	- 变量的取名规范 Naming
* 相对跳转 Relative Jump 
	- 位置无关代码 PIC (Position Independent Code)

## Lesson 4 [Judge a number odd or even](Lesson-4.md) 判断奇偶
* 条件分支 Condition 
	- 表达式求值  Expression Value
* 编码风格 Coding Style
	- 标识符命名 symbol naming
	- 代码缩进 (如果你知道自己在做什么，三层就足够了)
* 函数的传值和传址 Parameter's value and address
	- 程序二进制接口规范 ABI (Application Binary Interface)

## Lesson 5 [Summarize all numbers from 1 to 100](Lesson-5.md) 从1加到100求和
* for 循环 
	- 两种循环用法比较
* 自动变量 auto variable
	- C 语言的发展变迁 Old Style C/C89/C99/GNU C	
* 预处理过程 Pre-compile 
	- 条件编译
	- \# 和 \#\# 的用法
* DEBUG 调试宏
	- \_\_func\_\_, \_\_FUNCTION\_\_
	- \_\_LINE\_\_ 	
	- args... 和 \#\#args 的用法
		
## Lesson 6 [Print 9\*9 multiplication table](Lesson-6.md) 乘法表
* 循环嵌套
	- 两重循环的典型用法
	- break 和 continue 
* 程序的调试
	- 编译时和运行时错误
* 函数栈 Function Stack
	- 栈帧 Stack Frame
		
## Lesson 7 [Find the max prime number within 100](Lesson-7.md) 求100以内的最大素数
* 循环中的条件分支 
	- break 和 goto 用法	
* 数学库函数 math library
	- 静态链接和动态链接 static & dynamic linkage
* 算法效率 
	- 算法的时间复杂度分析 O(n) 
* 结构程序设计
	- 三种基本控制结构就可以写各种程序

# Intermediate Lessons
## Lesson 8 [Find 9 in number 1 to 100](Lesson-8.md) 1到100有多少个9
### 基本概念讲解
* 函数 Function
	- 函数的入口和出口
* 分解和分层 stratify 
	- 小即是美
* 过程抽象和接口设计 Procedure Abstract
	- 可复用的代码 Reuse
	- 接口小巧、简洁和正交
		
## Lesson 9 [Convert a number to a string](Lesson-9.md) 整型转字符串
### 基本概念讲解
* 字符数组 String and Character Array
	- 字符编码 ASCII 码表
* 字符串逆序 String Reverse 
	- 函数式宏定义 Function-like Macro
	
## Lesson 10 [Josephus ring](Lesson-10.md) 约瑟夫环
### 基本概念讲解
* 整型数组 Array	
	- 数组的初始化
* 数据结构和算法 DS & AL
	- 数据驱动编程 Data-Driven
	- 数据压倒一切，编程的核心是数据结构，而不是算法
* 链表思想 Link List
	- 算法优化 Optimization

## Lesson 11 [Calculate the distance between 2 points](Lesson-11.md) 求两个坐标点之间的距离
### 基本概念讲解
* 结构体 Struct
	- 结构体初始化
* 数组和结构体
	- 数组名参数的传址调用
	- 结构体参数的传值调用
* 复杂类型声明 typedef 
	- 预处理和编译时 Pre-compile & Compiling time
	- typedef 背后编译器的处理过程
* C99 中结构体的扩展用法
	- 驱动内核模块编写	
	
## Lesson 12 [Does your machine use little-endian?](Lesson-12.md) 判断机器存储是否小尾端
### 基本概念讲解
* 联合 Union
	- 存储分配
* 结构体空洞 Struct Hole
	- 对齐和填充 Alignment & Padding
* 数据的存储表示 Complements
	- 原码，反码和补码

## Lesson 13 [Sorry, your car is restricted today](Lesson-13.md) 对不起，你的车今天限行
### 基本概念讲解
* 分支语句 Switch
* 枚举用法 enum
	- 枚举类型的初始化
* 增量式开发 Incremental Development
	- 步步为营而不是一蹴而就
* 预定义宏的用法	
	- \_\_DATE\_\_ 
	- \_\_TIME\_\_
	
## Lesson 14 [Is there a way out?](Lesson-14.md) 判断地图上某点是否有出路
### 基本概念讲解
* 二维数组
	- 循环和分支
* 逻辑表达式 Logical Expression
	- 或 ||
	- 与 &&	
* 随机数生成 Random
	- 时间种子 Time seed
	

# Advanced Lessons

## Lesson 15 [Count bit 1 in a number](Lesson-15.md) 统计一个数二进制表示中1的个数
### 基本概念讲解
* 位操作
	- 移位 >>
	- 与 &
* 异或操作：
	- 按位加法	
* 算法效率
	- 过早优化是万恶之源
	- 先求运行，再求正确，最后求快
* 位域操作
	- 通过位域实现位操作
	- 嵌入式编程中的寄存器配置

## Lesson 16 [How to strcpy](Lesson-16.md) 字符串拷贝
### 基本概念讲解
* 指针
	- 计算机存储体系
* 动态内存分配 Memory Allocate	
	- heap & stack	
* assert 宏
	- 三元表达式
* 寻址和访存
	- 内存对齐
	- 防止编译器优化 volatile
	
## Lesson 17 [Count words in an artitle](Lesson-17.md) 统计单词个数
### 基本概念讲解
* 指针数组
	- 和二维数组的比较
* 动态内存分配
	- malloc & free
* 递归 Recursive 
	- 循环和递归 	
* 变量的生存期和作用域
	- static 用法
* 状态机思想的简单应用
	- state machine

## Lesson 18 [My printf](Lesson-18.md) 实现 printf
### 基本概念讲解
* 字符指针数组	
* 可变长度参数的函数实现
	- 字符串常量 const char *
	- ... 可变参数的用法
* 栈帧的应用
	- va_list 
	- va_start
	- va_arg
	- va_end

## Lesson 19 [Shell command parser](Lesson-19.md) 命令解释器
### 基本概念讲解
* 函数指针
	- 回调函数 Call-Back Function
* main 参数 argc, argv
	- 字符指针数组 vs 指针的指针
* 进程的环境变量
	- 进程栈空间布局
* 函数指针数组
	- 结构体数组
* 策略和机制分离
	- 高内聚低耦合原则

## Lesson 20 [Preprocessor](Lesson-20.md) 预处理器实现
### 基本概念讲解
* C语言去注释问题
	- 状态的变迁 20.1
	- 状态机编程模型1(if-else) 20.2
* 去多余空格问题 
	- Unix 编程艺术之表示原则: 把知识叠入数据以求逻辑质朴而健壮。
	- 字节流处理: 重定向和管道 
	- 状态机编程模型2(状态迁移表和函数指针数组) 20.3
* 宏定义替换问题
	- #define 
	- 状态机的设计思路和设计过程 20.4
	- 状态机的编程实现过程 20.5
* 条件编译问题
	- #if/#endif 
	- 实现代码分析 20.6

## Lesson 21 [Lexical analysis](Lesson-21.md) 词法分析器实现
### 基本概念讲解
* flex 词法分析器生成工具
	- lex.l 文件介绍
	- yy_nxt 数组
	- yy_accept 数组

* 词法分析器实现
	- 如何使用 yy_nxt 和 yy_accept
	- 词法匹配时的状态判别 


# Homework Projects
	
**The next 3 lessons are projects you should do it by yourself.**

## Lesson 22 [Guess number in my hand](Lesson-22.md) 猜数游戏
### 问题描述
猜数游戏：电脑随机产生4位数，然后用户输入4位数，电脑告诉你是?A?B，请你最后猜出电脑的4位数是多少？	
(4位数字互不重复，A表示位置和数字都对，B表示位置不对，数字对)


## Lesson 23 [Five-Chess game](Lesson-23.md) 五子棋
### 问题描述
五子棋：在一个9x9的棋盘上通过两人对弈的形式，依次在棋盘上放置两种颜色的棋子，哪一方先让五个棋子形成一条直线（包括横、竖、对角线3个方向），即为获胜。
(实现一个计算机下棋算法，让你的同组成员无法胜出，则算你赢)


## Lesson 24 [Build a simple Search Engenine](Lesson-24.md) 简单搜索引擎
### 问题描述
简单搜索引擎：从网页文件中抓取正文文本 (例如 "\<p\>hello, lumit.\</p\>" )，搜索是否存在用户输入的关键字 lumit，并返回相关段落正文。
同时从网页文件中抓取超链接URL (例如 \<a href="http://www.lumit.org">lumit - let us make it together.\</a\> )，并下载相关网页文件。依此递归。



