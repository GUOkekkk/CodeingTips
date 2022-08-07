# CodeingTips
This `.md` file is created to record some tips I met during the coding. I hope it could be my first blog and I can update it regularly and modify it clearer and more beautiful. But sorry for now it is only a chinese version.

这个`.md`文档是用来记录一些我遇到到问题，代码语法和方法在我写代码的时候（感觉中文退步太多）。。。我也想把他作为我的第一个blog并且持续更新，也需要继续学习让他越来越美观。有写blog的想法主要是受这位大神启发 https://doublelll3.ml/ 。BTW希望我能顺利找到工作。。。

## Markdown语法Tips
#### 如何打出代码框
使用 `` 反引号 ex：`.md`

#### 如何在Github的md文件里面使用LaTex
在Chrome浏览器上使用MathJax插件。

#### 如何换行
在`.md`文件中换行需要使用两次空格加回车
## Leetcode Tips
#### 线段树(Segment Tree)

## LaTex语法Tips
#### 如何打欧元符号
引用\usepackage{textcomp} 使用\texteuro

#### 不对称分段
引用\usepackage{paracol} 使用  
\columnratio{0.3}
\begin{paracol}{2}

\switchcolumn

\end{paracol}


## 数学
真的感觉数学太重要了，好多代数的知识都还给老师了。。。
#### 克罗内克积（张量积 or 外积）
首先是简单的向量的外积, ex：

$$ a = [a_1\ \  a_2]^T \ \ \ \ b = [b_1\  b_2 \ b_3] $$
$$a \otimes b = \begin{bmatrix} a_1b_1 & a_1b_2 & a_1b_3 \\ 
a_2b_1 & a_2b_2 & a_2b_3 \end{bmatrix}$$


也可以推广到矩阵形式，从外积推广到克罗内克积。  
如果$A$是一个$m \times n$的矩阵， 而$B$是一个$p \times q$的矩阵，则$ A \otimes B$是一个$mp \times nq$的分块矩阵

$$ A \otimes B = \begin{bmatrix} a_{11}B & \cdots & a_{1n}B \\ 
\vdots & \ddots & \vdots \\
a_{m1}B & \cdots & a_{mn}B \end{bmatrix} $$

#### 叉乘矩阵
