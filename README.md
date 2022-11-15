# CodeingTips
This `.md` file is created to record some tips I met during the coding. I hope it could be my first blog and I can update it regularly and modify it clearer and more beautiful. But sorry for now it is only a chinese version.

这个`.md`文档是用来记录一些我遇到到问题，代码语法和方法在我写代码的时候（感觉中文退步太多）。。。我也想把他作为我的第一个blog并且持续更新，也需要继续学习让他越来越美观。有写blog的想法主要是受这位大神启发 https://doublelll3.ml/ 。BTW希望我能顺利找到工作。。。


## Markdown语法Tips
### 如何打代码块
使用`tab`键
### 如何添加图片在md文档
1. 比较直接的方法就是把图片上传到repository中然后`![name](link)` 但是容易受DNS域名污染
2. 可以把图片转换到base64码再`![name](data:image/png;base64,XXX)` 但是base64码很长影响写作，可以`![name][base64str]`和`[base64str]:data:image/png;base64,XXX`来代替。`Png2Base64.ipynb`可以用来转换图片到base64码基于python。
Tip：但是不知道为什么我的第二种方法并不成功，第一种方法本地也没办法看到图片，只能用手机才能看到。

### 解决看不到自己的readme中的图片
DNS域名污染， 解决办法：
https://segmentfault.com/a/1190000038705840
### 如何打出代码框
使用 `` 反引号 ex：`.md`

### 如何在Github的md文件里面使用LaTex
在Chrome浏览器上使用MathJax插件。而且使用独立公式时需要和上下文各分开一行。使用换行符的时候也需要换行。

### 如何换行
在`.md`文件中换行需要使用两次空格加回车

### Github页面的一些快捷键
https://docs.github.com/cn/get-started/using-github/keyboard-shortcuts

### Github上生成Markdown文件的目录
Github上没办法使用`[TOC]`...真的是挺不智能的。  
使用VSCode中的Markdown All in One这个插件可以自动生成，考虑目前我的Blog还是没有太多内容，之后再创建目录吧。

## Leetcode Tips
### 线段树(Segment Tree)

## LaTex语法Tips
### 如何打欧元符号
引用\usepackage{textcomp} 使用\texteuro

### 不对称分段
引用\usepackage{paracol} 使用  
\columnratio{0.3}
\begin{paracol}{2}

\switchcolumn

\end{paracol}

### 矩阵

```
$$
\begin{gathered}
\begin{matrix} 0 & 1 \\ 
1 & 0 \end{matrix}
\quad
\begin{pmatrix} 0 & -i \\
i & 0 \end{pmatrix}
\quad
\begin{bmatrix} 0 & -1 \\ 
1 & 0 \end{bmatrix}
\quad
\begin{Bmatrix} 1 & 0 \\
0 & -1 \end{Bmatrix}
\quad
\begin{vmatrix} a & b \\ 
c & d \end{vmatrix}
\quad
\begin{Vmatrix} i & 0 \\ 
0 & -i \end{Vmatrix}
\end{gathered}
$$
```


$$
\begin{gathered}
\begin{matrix} 0 & 1 \\ 
1 & 0 \end{matrix}
\quad
\begin{pmatrix} 0 & -i \\ 
i & 0 \end{pmatrix}
\quad
\begin{bmatrix} 0 & -1 \\ 
1 & 0 \end{bmatrix}
\quad
\begin{Bmatrix} 1 & 0 \\
0 & -1 \end{Bmatrix}
\quad
\begin{vmatrix} a & b \\
c & d \end{vmatrix}
\quad
\begin{Vmatrix} i & 0 \\
0 & -i \end{Vmatrix}
\end{gathered}
$$


## 数学
真的感觉数学太重要了，好多代数的知识都还给老师了，愧对数学系。。。
### 克罗内克积（张量积/直积 or 外积）(Kronecker Product)
首先是简单的向量的外积, ex：

$$ a = [a_1\ \  a_2]^T \ \ \ \ b = [b_1\  b_2 \ b_3] $$
$$a \otimes b = \begin{bmatrix} a_1b_1 & a_1b_2 & a_1b_3 \\ 
a_2b_1 & a_2b_2 & a_2b_3 \end{bmatrix}$$


也可以推广到矩阵形式，从外积推广到克罗内克积。  
如果$A$是一个$m \times n$的矩阵， 而$B$是一个$p \times q$的矩阵，则$ A \otimes B$是一个$mp \times nq$的分块矩阵

$$ A \otimes B = \begin{bmatrix} a_{11}B & \cdots & a_{1n}B \\ 
\vdots & \ddots & \vdots \\
a_{m1}B & \cdots & a_{mn}B \end{bmatrix} $$

### 哈达玛积(Hadamard product)

### 矩阵乘法

### 叉乘矩阵

## 算法知识
最近准备大疆的感知算法工程师感觉还是很多基础知识需要补充学习, 而且很多的中文名字也需要对应一下。
### 本质矩阵(Essential Matrix)

## 快捷键
记录一些各种各样的快捷键。。。
+ `ctrl+F` 搜索  
+ `选中文件+F12` 修改文件名字  
+ 在Github页面使用`?`调出键盘快捷键
+ `ctrl+K` word里面插入超链接

## ROS2
### 如何保存数据--rosbag
Use `rosbag record` to store and `rosbag play` to read.


## Python
### pipreqs
生成`requirements.txt` 方便环境配置
在根目录下`pipreqs ./`
### list(reversed(list))
反转list
### python函数签名
就是告诉下面的函数我的输入输出是什么
`def find_path(slef, maze_3d: np.ndarray, start: list, stop: list) -> list`
### pycharm两次引号一次回车自动生成参数列表

### all() and any()
any(x)判断x对象是否为空对象，如果都为空、0、false，则返回false，如果不都为空、0、false，则返回true

ex:       ` if any(s < end and start < e for s, e in self.overlaps):
            return False`
            
note: 
+ 不能迭代tuple，只能变成array
+ any 里面的for loop 里面定义的s和e外部没办法调用
+  迭代器里任意一个为真就可以
            
all(x)如果all(x)参数x对象的所有元素不为0、’’、False或者x为空对象，则返回True，否则返回False

### plot大小不一样的子图以及控制坐标轴位置
            plt.figure()
            plt.rcParams['ytick.right'] = plt.rcParams['ytick.labelright'] = False
            plt.rcParams['ytick.left'] = plt.rcParams['ytick.labelleft'] = True
            plt.subplot(1,2,1)
            plt.plot(x, y,'r', label ='Trajectory')
            plt.xlabel('x')
            plt.ylabel('y')
            plt.legend(loc='upper left', fontsize=7)

            plt.rcParams['ytick.right'] = plt.rcParams['ytick.labelright'] = True
            plt.rcParams['ytick.left'] = plt.rcParams['ytick.labelleft'] = False
            plt.subplot(2,2,2)
            plt.plot(time, x,'b')
            plt.xlabel('time')
            plt.ylabel('x')


            plt.subplot(2,2,4)
            plt.plot(time, y,'b')
            plt.xlabel('time')
            plt.ylabel('y')

            plt.savefig('tra.png')
### JupyterTips
#### 使用`esc+f`进入查找替换
#### 长按`alt`加移动鼠标多行修改代码
