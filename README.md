# CodeingTips
This `.md` file is created to record some tips I met during the coding. I hope it could be my first blog and I can update it regularly and modify it clearer and more beautiful. But sorry for now it is only a chinese version.

这个`.md`文档是用来记录一些我遇到到问题，代码语法和方法在我写代码的时候（感觉中文退步太多）。。。我也想把他作为我的第一个blog并且持续更新，也需要继续学习让他越来越美观。有写blog的想法主要是受这位大神启发 https://doublelll3.ml/ （好像进不去了。。。）。BTW希望我能顺利找到工作。。。 

对NLP感兴趣的也可以看看这个博主的博客 https://ivenwang.com/timeline/ 这个博主这种总结积累的过程真的很值得学习
- [CodeingTips](#codeingtips)
  - [Ubuntu](#ubuntu)
    - [ln](#ln)
    - [mkdir](#mkdir)
    - [cd](#cd)
    - [rm](#rm)
    - [pwd](#pwd)
    - [vi的用法](#vi的用法)
  - [Docker用法](#docker用法)
  - [Git](#git)
    - [Git push时，远端和本地同时修改](#git-push时远端和本地同时修改)
    - [git clone --recursive](#git-clone---recursive)
    - [git checkout](#git-checkout)
    - [git log + q](#git-log--q)
    - [git branch -a](#git-branch--a)
  - [Markdown语法Tips](#markdown语法tips)
    - [如何打代码块](#如何打代码块)
    - [如何添加图片在md文档](#如何添加图片在md文档)
    - [解决看不到自己的readme中的图片](#解决看不到自己的readme中的图片)
    - [如何打出代码框](#如何打出代码框)
    - [如何在Github的md文件里面使用LaTex](#如何在github的md文件里面使用latex)
    - [如何换行](#如何换行)
    - [Github页面的一些快捷键](#github页面的一些快捷键)
    - [Github上生成Markdown文件的目录](#github上生成markdown文件的目录)
  - [Leetcode Tips](#leetcode-tips)
    - [线段树(Segment Tree)](#线段树segment-tree)
  - [LaTex语法Tips](#latex语法tips)
    - [用`mininpage`插入图片（例如生成图片抬头）](#用mininpage插入图片例如生成图片抬头)
    - [如何打欧元符号](#如何打欧元符号)
    - [不对称分段](#不对称分段)
    - [表格](#表格)
    - [矩阵](#矩阵)
  - [数学](#数学)
    - [克罗内克积（张量积/直积 or 外积）(Kronecker Product)](#克罗内克积张量积直积-or-外积kronecker-product)
    - [哈达玛积(Hadamard product)](#哈达玛积hadamard-product)
    - [矩阵乘法](#矩阵乘法)
    - [叉乘矩阵](#叉乘矩阵)
    - [Mahalanobis distance](#mahalanobis-distance)
  - [算法知识](#算法知识)
    - [本质矩阵(Essential Matrix)](#本质矩阵essential-matrix)
    - [基本矩阵(Fundamental Matrix)](#基本矩阵fundamental-matrix)
    - [单应矩阵(Homograph Matrix)](#单应矩阵homograph-matrix)
    - [Levenberg-Marquardt Algorithm](#levenberg-marquardt-algorithm)
    - [Iteratively Rewighted Least Squares](#iteratively-rewighted-least-squares)
    - [EndtoEnd learning](#endtoend-learning)
    - [Covisibility Graph](#covisibility-graph)
  - [快捷键](#快捷键)
  - [ROS2](#ros2)
    - [如何保存数据--rosbag](#如何保存数据--rosbag)
  - [Python](#python)
    - [使用glob或者os.listdir来得到文件夹中的文件地址](#使用glob或者oslistdir来得到文件夹中的文件地址)
    - [tqdm](#tqdm)
    - [交换两个list中的元素](#交换两个list中的元素)
    - [内置函数](#内置函数)
    - [Lambda函数](#lambda函数)
    - [String](#string)
    - [JSON](#json)
    - [TensorFlow 2.0](#tensorflow-20)
      - [以前的学习笔记](#以前的学习笔记)
      - [TF常用函数](#tf常用函数)
    - [Numpy](#numpy)
    - [一个有趣的np的sort](#一个有趣的np的sort)
      - [在 sort 函数中排序字段](#在-sort-函数中排序字段)
    - [Pandas](#pandas)
      - [读取](#读取)
      - [随机生成DF](#随机生成df)
      - [按条件搜索](#按条件搜索)
      - [groupby函数](#groupby函数)
    - [pipreqs](#pipreqs)
    - [list(reversed(list))](#listreversedlist)
    - [python函数签名](#python函数签名)
    - [pycharm两次引号一次回车自动生成参数列表](#pycharm两次引号一次回车自动生成参数列表)
    - [all() and any()](#all-and-any)
    - [plot大小不一样的子图以及控制坐标轴位置](#plot大小不一样的子图以及控制坐标轴位置)
  - [C++](#c)
    - [-\> and .](#--and-)
    - [～A()](#a)
  - [JupyterTips](#jupytertips)
    - [使用`esc+f`进入查找替换](#使用escf进入查找替换)
    - [长按`alt`加移动鼠标多行修改代码](#长按alt加移动鼠标多行修改代码)


## Ubuntu
### 在Ubuntu下面修改鼠标侧键
    sudo apt install xbindkeys xautomation
    xbindkeys --defaults > $HOME/.xbindkeysrc
检测侧键 

    xev | grep button
    nano ~/.xbindkeysrc
命令 

    #CTRL + C
    "xte 'keydown Control_L' 'key c' 'keyup Control_L'"
    b:9

    #CTRL + V
    "xte 'keydown Control_L' 'key v' 'keyup Control_L'"
    b:8
### ln
复制一个链接到另一个地址 ln -s（软复制）用ls查看时有～标志

### mkdir
### cd
### rm
rm -r 删除整个文件夹

### pwd
输出当前路径

### vi的用法(nano is better)
https://www.cnblogs.com/emanlee/archive/2011/11/10/2243930.html

## Docker用法
https://www.quanxiaoha.com/docker/docker-container.html

## Git
### Git push时，远端和本地同时修改
先git pull再进行add, commit再git push

### git clone --recursive
### git checkout 
### git log + q
### git branch -a

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
### 用`mininpage`插入图片（例如生成图片抬头）
            \begin{minipage}[b]{0.6\linewidth}
            \includegraphics[height=1.5cm, width=3.8cm]{Figures/LogoECN.png}
            \end{minipage}
            \begin{minipage}[b]{0.35\linewidth}
            \includegraphics[height=1.5cm, width=5cm]{Figures/vblogo.png}
            \end{minipage}
### 如何打欧元符号
引用\usepackage{textcomp} 使用\texteuro

### 不对称分段
引用\usepackage{paracol} 使用  
\columnratio{0.3}
\begin{paracol}{2}

\switchcolumn

\end{paracol}

### 表格
            \usepackage{tabularx}
            \usepackage{booktabs}

            \setlength\tabcolsep{7pt} % Adjust column spacing
            \begin{table}[h]\centering
            \caption{Different packages related in SLAM on ROS}
            \begin{tabularx}{\textwidth}{lXXX}\toprule
             & Merits & Demerits & Principle\\\midrule
            HectorSLAM & No need for odometer,high accuracy & Need a laser scanner with high update frequency and low measurement noise
             & Scan-matching (Gaussian-Newton equation)
            \\\midrule
            KartoSLAM
             & Have a better performance when drawing in a larger environment & Require a large memory to store nodes & Spare Pose Adjustment(SPA)\\\midrule
            3D\_SLAM
             & Build a 3D map and get more information
             & Need a 3D lidar and better cpu to support a lot of calculations & Point-to-Plane (Iterative Closest Point)\\\midrule

            GmappingSLAM & high accuracy in a \newline small environment,  low requirement for the scanning frequency of the lidar
             & Need a lot of particle simulations to get good results
             &  Rao-Blackwellized particle filter
            \\\bottomrule
            \label{slam}
            \end{tabularx}
            \end{table}

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
### Hamilton Product for the quaternion multiplication
### Mahalanobis distance
### Spherical Harmonics & Spherical Gaussian
都是一种球面基函数，用来表示另一个复杂的非线性函数 

Spherical Harmonics：球谐函数， 球面坐标系下的基函数来源于Laplace方程的解，正交，旋转不变性 一阶1一个系数，二阶4个系数，三阶九个系数（常用） 

Laplace方程：Laplace算子，二阶偏导和为0, 如果等于一个函数就是Poisson方程（最基础的椭圆方程） 

Spherical Gaussian：在球面上服从Gauss分布的基函数，可以自由设计 

球面坐标系：可以用颜色也可以用形状来表示一个函数，所以为什么用基函数来表示光照情况， 

三维空间下的一种坐标系，就像二维的极坐标系，三维空间常见坐标系：直角坐标系，圆柱坐标系

## 算法知识
最近准备大疆的感知算法工程师感觉还是很多基础知识需要补充学习, 而且很多的中文名字也需要对应一下。 
### 本质矩阵(Essential Matrix)
### 基本矩阵(Fundamental Matrix)
### 单应矩阵(Homograph Matrix)
https://blog.csdn.net/kokerf/article/details/72191054

### Levenberg-Marquardt Algorithm
### Iteratively Rewighted Least Squares
### EndtoEnd learning
不提取数据特征，让模型自己去学习数据。

### Covisibility Graph
https://www.cnblogs.com/liuzhenbo/p/10849840.html

### 距离场
场函数，空间中任意一个点到附近标志物的最小距离 有正有负表示内部或外部

### 深度学习的一些评价标准
Recall： TP/（TP + FN）查全 是不是所有的正样本都被检测出来： 肿瘤 

Precision：TP/（TP + FP）查准 输出的正样本是不是正确：垃圾邮件 

mAP： mean average precision 针对目标检测（也用IoU判断） 计算PR曲线下面的面积再根据类别平均
https://zhuanlan.zhihu.com/p/43068926

IoU：intersection over union 针对语义分割  

PQ：Panoptic Segmentation 针对全景分割 

### Attention
https://zhuanlan.zhihu.com/p/392553460
#### Self Attention
#### Multi-head attention

### NLP中的Mask操作
1.为了计算中处理那些补出来的0的信息 

2.在decoder中去掉一些文本中的本来的信息，加强训练避免后续分词的影响 

### Operator
#### Sobel 一阶微分 过滤模糊的地方
#### Laplace 二阶微分
#### LOG 先Gauss滤波再Laplace算子

### ICP
Using the SVD to get the soulution  

Optimize:
- Filter some outlier which is the noise during the data collection
- Use the KDtree structure to save the time

### DLT
利用叉乘来解决PnP中的尺度不确定性问题（因为尺度不确定不能用最小二乘法）

### 对极约束
对两张2d图像求解T的方法，通过八对点方法，求解E或者F

### PnP问题
已知3D点和对应2d点来求解T，可以用三对点就解决，外加一对点验证. 

具体方法有EPnP，DLT等

### ICP方法
3D和3D来求解T，2dto2d应该也可以，比较困难知道匹配关系. 

可以用SVD或者BA来求解

### BA
更多是后段全局优化，最小二乘法收敛光束

### RANSAC
Random Sample Consensus是一种过滤outlier的方法 
- 选择子集
- 建立模型
- 确定ouliter或者inlier
- 迭代
- 找到最多inlier的集合

### RTK
Real Time Kinematic技术，基于GPS技术（四颗卫星，一颗消除时间误差， 四个参数）可以得到PVT（Position Velocity and Time）

GPS误差比较大1m以上， 用RTK减少误差（通过自身定位信息和基准站的相对定位信息来求解误差，使用实时差分），更为通用的是网络RTK生成虚拟基准站，需要移动网络

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
### 使用glob或者os.listdir来得到文件夹中的文件地址
但是需要注意的是，读取出来的文件是无序的。需要用`list.sort(key = lambda x : int(x.split('something')[0])` 
这个sort没有返回值，需要注意

### tqdm
一个package可以可视化一个迭代器

### 交换两个list中的元素
a, b = b, a
### 内置函数
常用内置函数 https://www.runoob.com/python/python-built-in-functions.html  

`filter(function, iterable):` 过滤序列，true or false function  

`map(function, iterable, ...):` 对一个或多个子列操作 ex：`map(lambda x, y: x + y, [1, 3, 5, 7, 9], [2, 4, 6, 8, 10])` 
### Lambda函数
https://www.runoob.com/python/python-built-in-functions.html
            # 程序从列表中过滤出偶数项
            my_list = [1, 5, 4, 6, 8, 11, 3, 12]

            new_list = list(filter(lambda x: (x%2 == 0) , my_list))

            print(new_list)
`lambda`和`filter`结合
### String
使用`str.split(' ', num)`分割。

            string="asdasd"
            print(list(string))
            string_two=list(string)
            print("".join(string_two))
全部分割

            str.isdigit()    判断所有字符都是数字（整形）   

            str.isalnum() 判断所有字符都是数字或者字母    

            str.isalpha()  判断所有字符都是字母 

            str.islower()  判断所有字符都是小写 

            str.isupper() 判断所有字符都是大写

            str.istitle()    判断所有单词都是首字母大写
### JSON
Json是JavaScript Object Notation是一种轻量级的数据交换格式. 

需要使用`json`这个包来操作。 存在`json.loads`（处理字符串）和`json.load`（处理类文件对象）两种函数。 

可以将`json`和`pandas`结合起来使用。https://geek-docs.com/pandas/pandas-read-write/pandas-reading-and-writing-json.html  
使用`frame = pd.DataFrame 
frame.to_json('.json')`

### TensorFlow 2.0
#### 以前的学习笔记
https://github.com/GUOkekkk/TensorFlowLearn
#### TF常用函数
### Numpy
Numpy基本函数 https://cloud.tencent.com/developer/article/1770104
### 一个有趣的np的sort
#### 高维数组最好还是用a[np.argsort[:, 1]]
#### 在 sort 函数中排序字段 
            dt = np.dtype([('name',  'S10'),('age',  int)]) 
            a = np.array([("raju",21),("anil",25),("ravi",  17),  ("amar",27)], dtype = dt)  
            print ('我们的数组是：')
            print (a)
            print ('\n')
            print ('按 name 排序：')
            print (np.sort(a, order =  'name'))

### Pandas
和SQL基本上一致，Pandas的Series是一列，多个列组成为一个DataFrame。

前面的数字为index，也可以自己修改为str或者其他。

https://zhuanlan.zhihu.com/p/113342292 Pandas的一些计数用法。`str.count`

https://zhuanlan.zhihu.com/p/340770847 Pandas的`apply`用法。
#### 读取

            data['w']  #选择表格中的'w'列，使用类字典属性,返回的是Series类型

            data.w    #选择表格中的'w'列，使用点属性,返回的是Series类型

            data[['w']]  #选择表格中的'w'列，返回的是DataFrame属性

            data[['w','z']]  #选择表格中的'w'、'z'列

            data[0:2]  #返回第1行到第2行的所有行，前闭后开，包括前不包括后

            data[1:2]  #返回第2行，从0计，返回的是单行，通过有前后值的索引形式，
                   #如果采用data[1]则报错

            data.ix[1:2] #返回第2行的第三种方法，返回的是DataFrame，跟data[1:2]同

            data['a':'b']  #利用index值进行切片，返回的是**前闭后闭**的DataFrame, 
                    #即末端是包含的  
            data.irow(0)   #取data的第一行
            data.icol(0)   #取data的第一列

            data.head()  #返回data的前几行数据，默认为前五行，需要前十行则dta.head(10)
            data.tail()  #返回data的后几行数据，默认为后五行，需要后十行则data.tail(10)

            ser.iget_value(0)  #选取ser序列中的第一个
            ser.iget_value(-1) #选取ser序列中的最后一个，这种轴索引包含索引器的series不能采用ser[-1]去获取最后一个，这回引起歧义。

            data.iloc[-1]   #选取DataFrame最后一行，返回的是Series
            data.iloc[-1:]   #选取DataFrame最后一行，返回的是DataFrame

            data.loc['a',['w','x']]   #返回‘a’行'w'、'x'列，这种用于选取行索引列索引已知

            data.iat[1,1]   #选取第二行第二列，用于已知行、列位置的选取

#### 随机生成DF
            company=["A","B","C"]
            ​
            data=pd.DataFrame({
                "company":[company[x] for x in np.random.randint(0,len(company),10)],
                "salary":np.random.randint(5,50,10),
                "age":np.random.randint(15,50,10)
            }
            )
#### 按条件搜索
`df[['key1', 'key2']][(df['key'] > 100) & | (df['key'] < 200)]`
#### groupby函数
`group = data.groupby("company")`
转换成多个分组的sunDF
`data.groupby('company').agg({'count'})`
计算每组的个数
`data.groupby('company').agg({'salary':'median','age':'mean'})` 
对分组了的数据进行agg操作
`data['avg_salary'] = data.groupby('company')['salary'].transform('mean')` 
使用transform简便操作
`oldest_staff = data.groupby('company',as_index=False).apply(get_oldest_staff)`

             def get_oldest_staff(x):
                 df = x.sort_values(by = 'age',ascending=True)
               return df.iloc[-1,:]
使用apply传入custom函数
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
            



## C++
### -> and .
-> 当对象是指针类型时使用 

. 当对象是实体

### ～A()
Destroctor

## JupyterTips
### 使用`esc+f`进入查找替换
### 长按`alt`加移动鼠标多行修改代码
