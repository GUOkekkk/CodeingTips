# CodeingTips
This `.md` file is created to record some tips I met during the coding. I hope it could be my first blog and I can update it regularly and modify it clearer and more beautiful. But sorry for now it is only a chinese version.
这个`.md`文档是用来记录一些我遇到到问题，代码语法和方法在我写代码的时候（感觉中文退步太多）。。。我也想把他作为我的第一个blog并且持续更新，也需要继续学习让他越来越美观。有写blog的想法主要是受这位大神启发 https://doublelll3.ml/ （好像进不去了。。。）。BTW希望我能顺利找到工作。。。

对NLP感兴趣的也可以看看这个博主的博客 https://ivenwang.com/timeline/ 这个博主这种总结积累的过程真的很值得学习

积累确实是一个好的事情，但是感觉有时候会耽误进程，还是慢慢做再慢慢调整。看见各种bloger和vloger感觉真的是有意思，但是让我自己做又觉得好麻烦。就把这个网页做为一个简单的blog记录一下遇到的问题和解决方案吧（主要是给自己。。），总结一下遇到的问题确实是很有帮助的，还有[文献](https://github.com/GUOkekkk/Literature)总结。

🤖 : Optimistic science fiction typically imagines a future where humans create art and pursue fulfilling pastimes while AI-enabled robots handle dull or dangerous tasks. In contrast, the AI systems of today display increasingly sophisticated generative abilities on ostensible creative tasks. But where are the robots? This gap is known as Moravec’s paradox, the thesis that the hardest problems in AI involve sensorimotor skills, not abstract thought or reasoning. To put it another way, “**The hard problems are easy, and the easy problems are hard.**”

如果有侵权请直接联系[我](guoke9612@gmail.com)，我会立马删除.

If there is any infringement, please feel free to contact [me](guoke9612@gmail.com) directly, I will delete it immediately

- [CodeingTips](#codeingtips)
  - [一些好的总结](#一些好的总结)
    - [SLAM benchmark](#slam-benchmark)
    - [pointcloud place recognition](#pointcloud-place-recognition)
    - [Object Pose Estimation](#object-pose-estimation)
    - [Robot Academy](#robot-academy)
    - [DL Visualization](#dl-visualization)
    - [Robot simulation \& Robot learning](#robot-simulation--robot-learning)
      - [Sim2Real](#sim2real)
      - [Robot long-term learning](#robot-long-term-learning)
  - [工作流程](#工作流程)
      - [Server \& Training](#server--training)
      - [Git merge](#git-merge)
  - [Windows11](#windows11)
    - [Make Win11 like Linux](#make-win11-like-linux)
    - [Don't use mouse!!! ⌨️](#dont-use-mouse-️)
  - [Ubuntu](#ubuntu)
    - [Don't use mouse!!! ⌨️](#dont-use-mouse-️-1)
    - [set up](#set-up)
    - [Ubuntu 22.04 change the workspace](#ubuntu-2204-change-the-workspace)
    - [count how many files in the current folder](#count-how-many-files-in-the-current-folder)
    - [record the screen](#record-the-screen)
    - [ffmpeg](#ffmpeg)
    - [sudo nautilus](#sudo-nautilus)
    - [脚本语言/Shell](#脚本语言shell)
    - [Use Terminator](#use-terminator)
    - [zsh美化终端，但是会有点慢](#zsh美化终端但是会有点慢)
    - [tmux](#tmux)
    - [history ｜ grep](#history--grep)
    - [draw.io](#drawio)
    - [登陆进去黑屏但是cursor可以用](#登陆进去黑屏但是cursor可以用)
    - [Ubuntu重启](#ubuntu重启)
    - [use Jekyll in local](#use-jekyll-in-local)
    - [在Ubuntu下面修改鼠标侧键](#在ubuntu下面修改鼠标侧键)
    - [python and python3](#python-and-python3)
    - [ln](#ln)
    - [mv](#mv)
    - [删除目录下特定文件名文件](#删除目录下特定文件名文件)
    - [import bashrc to zshrc](#import-bashrc-to-zshrc)
    - [check python env](#check-python-env)
    - [check code lines](#check-code-lines)
    - [dvc](#dvc)
    - [cp](#cp)
      - [copy from the server](#copy-from-the-server)
    - [mkdir](#mkdir)
    - [cd](#cd)
    - [rm](#rm)
    - [du -hs \*](#du--hs-)
    - [pwd](#pwd)
    - [vi的用法(nano is easier)](#vi的用法nano-is-easier)
      - [use '?' to search and 'n' for the next](#use--to-search-and-n-for-the-next)
  - [VScode](#vscode)
    - [Auto-form does not work](#auto-form-does-not-work)
    - [Keyshot in Linux](#keyshot-in-linux)
    - [Server error](#server-error)
    - [Pylint to check Python code form](#pylint-to-check-python-code-form)
    - [Debug](#debug)
  - [Docker用法](#docker用法)
    - [A small example of the docker](#a-small-example-of-the-docker)
        - [Build the image](#build-the-image)
        - [Build the container](#build-the-container)
    - [docker debug](#docker-debug)
        - [reboot](#reboot)
    - [Can not see the plot in dokcer container](#can-not-see-the-plot-in-dokcer-container)
    - [Enter the container](#enter-the-container)
  - [ChatGPT Prompts](#chatgpt-prompts)
  - [Git](#git)
    - [Atomic Git Commit](#atomic-git-commit)
    - [Git push时，远端和本地同时修改](#git-push时远端和本地同时修改)
    - [Git修改commit](#git修改commit)
    - [git pull does not work](#git-pull-does-not-work)
    - [git clone --recursive](#git-clone---recursive)
    - [git checkout](#git-checkout)
    - [git log + q](#git-log--q)
    - [git branch -a](#git-branch--a)
    - [Git permission denied](#git-permission-denied)
    - [git delete](#git-delete)
  - [Markdown语法Tips](#markdown语法tips)
    - [Emojipeida](#emojipeida)
    - [Cheatsheet](#cheatsheet)
    - [md标题没办法引到外部连接](#md标题没办法引到外部连接)
    - [生成requirement和项目结构](#生成requirement和项目结构)
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
    - [偏微分和偏导数](#偏微分和偏导数)
    - [克罗内克积（张量积/直积 or 外积）(Kronecker Product)](#克罗内克积张量积直积-or-外积kronecker-product)
    - [哈达玛积(Hadamard product)](#哈达玛积hadamard-product)
    - [矩阵乘法](#矩阵乘法)
    - [叉乘矩阵](#叉乘矩阵)
    - [Hamilton Product for the quaternion multiplication](#hamilton-product-for-the-quaternion-multiplication)
    - [Mahalanobis distance](#mahalanobis-distance)
    - [Frobenius norm](#frobenius-norm)
    - [Spherical Harmonics \& Spherical Gaussian](#spherical-harmonics--spherical-gaussian)
    - [KL散度/相对熵](#kl散度相对熵)
    - [Grobner basis](#grobner-basis)
    - [SVD](#svd)
    - [Pareto front \& Nash equilibrium](#pareto-front--nash-equilibrium)
    - [变换](#变换)
    - [Normalization \& Standardization](#normalization--standardization)
    - [有偏估计和无偏估计（方差）](#有偏估计和无偏估计方差)
    - [Convex \& Concave](#convex--concave)
  - [算法知识](#算法知识)
    - [四元数 旋转矩阵 旋转向量 欧垃角](#四元数-旋转矩阵-旋转向量-欧垃角)
      - [quaternion](#quaternion)
      - [rotation matrix](#rotation-matrix)
      - [rotation vector](#rotation-vector)
      - [Euler angle](#euler-angle)
    - [Activate function](#activate-function)
    - [梯度消失和爆炸](#梯度消失和爆炸)
    - [为什么要做normalization](#为什么要做normalization)
    - [pretrain \& fine-tuning](#pretrain--fine-tuning)
    - [GRU](#gru)
    - [VO](#vo)
      - [Feature-based Method](#feature-based-method)
      - [Direct method](#direct-method)
    - [Outlier Rejection](#outlier-rejection)
    - [CNN explainer](#cnn-explainer)
    - [常用矩阵](#常用矩阵)
    - [KM algorithm](#km-algorithm)
    - [对极约束的问题](#对极约束的问题)
    - [Levenberg-Marquardt Algorithm](#levenberg-marquardt-algorithm)
    - [Iteratively Rewighted Least Squares](#iteratively-rewighted-least-squares)
    - [EndtoEnd learning](#endtoend-learning)
    - [路径规划](#路径规划)
      - [RRT(Rapidly-exploring random tree)](#rrtrapidly-exploring-random-tree)
      - [PRM(Probabilistic Roadmap)(Dijkstra method)](#prmprobabilistic-roadmapdijkstra-method)
      - [A\*](#a)
      - [DWA](#dwa)
    - [TCN](#tcn)
    - [一些Clustering 方法](#一些clustering-方法)
    - [相似度计算](#相似度计算)
    - [Covisibility Graph](#covisibility-graph)
    - [距离场](#距离场)
    - [深度学习的一些评价标准](#深度学习的一些评价标准)
    - [Zero-shot learning \& few-shot learning](#zero-shot-learning--few-shot-learning)
    - [Using a fixed conv1D to replace the avg\_pool1D could reduce the time](#using-a-fixed-conv1d-to-replace-the-avg_pool1d-could-reduce-the-time)
    - [Variational Autoencoders](#variational-autoencoders)
    - [Transformer](#transformer)
      - [Attention](#attention)
      - [Key query, value](#key-query-value)
      - [Encoder-decoder](#encoder-decoder)
      - [Deep Double Descent](#deep-double-descent)
    - [Regularization](#regularization)
    - [Short-cut](#short-cut)
    - [NLP中的Mask操作](#nlp中的mask操作)
    - [Operator](#operator)
      - [Sobel 一阶微分 过滤模糊的地方](#sobel-一阶微分-过滤模糊的地方)
      - [Laplace 二阶微分](#laplace-二阶微分)
      - [LOG 先Gauss滤波再Laplace算子](#log-先gauss滤波再laplace算子)
    - [SLAM十四讲](#slam十四讲)
      - [面试题：](#面试题)
      - [笔记](#笔记)
    - [ICP](#icp)
    - [DLT-PnP](#dlt-pnp)
    - [对极约束](#对极约束)
    - [三角测量](#三角测量)
    - [PnP问题](#pnp问题)
    - [BA](#ba)
    - [Pose Graph](#pose-graph)
    - [RANSAC](#ransac)
    - [RTK](#rtk)
    - [BERT](#bert)
    - [pre-trained network](#pre-trained-network)
    - [Bearing Angle Image](#bearing-angle-image)
    - [DL+Transdisciplinary](#dltransdisciplinary)
    - [EKF](#ekf)
    - [Optical Flow](#optical-flow)
    - [常见的Feature（具体看笔记）](#常见的feature具体看笔记)
      - [Harris](#harris)
      - [FAST](#fast)
      - [BRIEF](#brief)
      - [ORB](#orb)
      - [SIFT](#sift)
      - [SURF](#surf)
    - [二叉树遍历](#二叉树遍历)
    - [ARP(Address Resolution Protocol)](#arpaddress-resolution-protocol)
    - [LIDAR \& RADAR](#lidar--radar)
    - [SLAM on ROS Comparison](#slam-on-ros-comparison)
    - [Exteroceptive \& Proprioceptive](#exteroceptive--proprioceptive)
  - [计算机基础](#计算机基础)
    - [解释型语言和编译型语言](#解释型语言和编译型语言)
    - [pyhon值传递和引用传递](#pyhon值传递和引用传递)
    - [C++指针传递和引用传递](#c指针传递和引用传递)
    - [Assert in Python](#assert-in-python)
    - [补码](#补码)
  - [快捷键](#快捷键)
  - [ROS2](#ros2)
    - [如何保存数据--rosbag](#如何保存数据--rosbag)
    - [Common bug](#common-bug)
    - [check the topic](#check-the-topic)
    - [Insttall packages](#insttall-packages)
  - [Python](#python)
    - [PEP 8 Coding Style](#pep-8-coding-style)
    - [Python常用运算符](#python常用运算符)
    - [Python Access](#python-access)
    - [Python argparse](#python-argparse)
    - [Breakpoint()](#breakpoint)
    - [Assert的用法](#assert的用法)
    - [args](#args)
    - [the product of the list](#the-product-of-the-list)
    - [阶乘](#阶乘)
    - [使用glob或者os.listdir来得到文件夹中的文件地址](#使用glob或者oslistdir来得到文件夹中的文件地址)
    - [If `import` does not work](#if-import-does-not-work)
    - [Pytorch3D](#pytorch3d)
    - [tqdm](#tqdm)
    - [ord()](#ord)
    - [join](#join)
    - [交换两个list中的元素](#交换两个list中的元素)
    - [内置函数](#内置函数)
    - [Lambda函数](#lambda函数)
      - [sort and lambda](#sort-and-lambda)
    - [String](#string)
      - [replace](#replace)
      - [split](#split)
      - [f-string](#f-string)
      - ["{}".format](#format)
    - [数位之和](#数位之和)
    - [JSON](#json)
    - [TensorFlow 2.0](#tensorflow-20)
      - [以前的学习笔记](#以前的学习笔记)
      - [TF常用函数](#tf常用函数)
    - [Numpy](#numpy)
      - [Numpy出现维度不对的时候用.ravel把二维变一维](#numpy出现维度不对的时候用ravel把二维变一维)
      - [\[ : : 2\]](#---2)
      - [np.sort](#npsort)
      - [在 np.sort 函数中排序字段](#在-npsort-函数中排序字段)
      - [np norm axis=i ,remove the i axis on the final result shape](#np-norm-axisi-remove-the-i-axis-on-the-final-result-shape)
      - [np查找满足条件的元素个数](#np查找满足条件的元素个数)
      - [np.where()用法](#npwhere用法)
      - [numpy插入一列](#numpy插入一列)
      - [np.set\_printoptions(threshold=1000)](#npset_printoptionsthreshold1000)
      - [过滤ndarrady中的重复元素](#过滤ndarrady中的重复元素)
      - [NP数组合并分割](#np数组合并分割)
      - [inverse the array](#inverse-the-array)
    - [Pandas](#pandas)
      - [读取](#读取)
      - [随机生成DF](#随机生成df)
      - [按条件搜索](#按条件搜索)
      - [groupby函数](#groupby函数)
    - [pipreqs](#pipreqs)
    - [list(reversed(list))](#listreversedlist)
    - [python函数签名](#python函数签名)
    - [pycharm两次引号一次回车自动生成参数列表](#pycharm两次引号一次回车自动生成参数列表)
    - [dict/hash table](#dicthash-table)
    - [define a sort rule in Python](#define-a-sort-rule-in-python)
    - [all() and any()](#all-and-any)
    - [A better way to get the attribute from the class](#a-better-way-to-get-the-attribute-from-the-class)
    - [Python map](#python-map)
    - [Opencv](#opencv)
      - [cv2只支持unit8\<0-255\>或者float32\<0.0-1.0\>](#cv2只支持unit80-255或者float3200-10)
      - [一个方便键盘控制的cv的小demo](#一个方便键盘控制的cv的小demo)
      - [Opencv不支持SURF](#opencv不支持surf)
      - [COLOR\_GRAY2BGR](#color_gray2bgr)
    - [Python传入和传出的参数最好还是不要\_开头](#python传入和传出的参数最好还是不要_开头)
    - [内部外部参数也需要注意](#内部外部参数也需要注意)
    - [super().__init__(paras)](#superinitparas)
    - [plot大小不一样的子图以及控制坐标轴位置](#plot大小不一样的子图以及控制坐标轴位置)
    - [Add legends elegantly](#add-legends-elegantly)
    - [Python Union](#python-union)
    - [Python Debug mode](#python-debug-mode)
    - [PyTorch](#pytorch)
    - [循环生成网络的层](#循环生成网络的层)
      - [.to(device=device)](#todevicedevice)
      - [.cpu() \& .cuda()](#cpu--cuda)
      - [torch.matmul()](#torchmatmul)
      - [summary](#summary)
      - [.squeeze and .unsqueeze](#squeeze-and-unsqueeze)
      - [cat the iterative tensor](#cat-the-iterative-tensor)
      - [torch乘法](#torch乘法)
      - [Inplace???](#inplace)
    - [Python训练加速](#python训练加速)
  - [C++](#c)
    - [size\_t](#size_t)
    - [-\> and .](#--and-)
    - [A good example to filter the data](#a-good-example-to-filter-the-data)
    - [～A()](#a-1)
  - [JupyterTips](#jupytertips)
    - [使用`esc+f`进入查找替换](#使用escf进入查找替换)
    - [长按`alt`加移动鼠标多行修改代码](#长按alt加移动鼠标多行修改代码)






## 一些好的总结
### SLAM benchmark
https://www.cnblogs.com/kin-zhang/p/16943210.html
### pointcloud place recognition
https://github.com/kxhit/awesome-point-cloud-place-recognition
### Object Pose Estimation
https://github.com/YoungXIAO13/ObjectPoseEstimationSummary
### Robot Academy
https://robotacademy.net.au/
### DL Visualization
https://jalammar.github.io/illustrated-word2vec/
### Robot simulation & Robot learning
https://github.com/zalo/mujoco_wasm
#### Sim2Real
https://zhuanlan.zhihu.com/p/510951914
#### Robot long-term learning
https://ai.facebook.com/blog/robots-learning-video-simulation-artificial-visual-cortex-vc-1/

## 工作流程
#### Server & Training
- 连接server `ssh servername`
- 在`Dockerfile`里创建image `sudo -H docker build - <torch_gk_pnp_Dockerfile  -t nash_pnp`
- 通过image创建container `docker run --name torch-pnp --shm-size=16gb --gpus all -it -v /data:/data -v /home/ke:/workspace --privileged -e DISPLAY=$DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix --env PYTHONPATH=/workspace/torch_pnp/alopix:/workspace/torch_pnp/alovb:/workspace/torch_pnp/aloception-oss:/workspace/torch_pnp/alovb/alovb/pnp_transformer nash_pnp`
- check the nivida `watch -n 0.1 nvidia-smi` & choose the suitable GPU device `export_CUDA_VISIBLE_DEVICES=0`
- 进入container连接WandB `--log`
- 开始training `add some args`
- check the memory `du -hs *`
- check the pid `ps -aux | grep -v grep | grep 1409800`
- show the image `ssh -X vb-4` and `docker run --name torch-pnp --shm-size=16gb --net=host --gpus all -it -v /data:/data -v /home/ke:/workspace -v /home/ubuntu/weights:/weights --privileged -e DISPLAY=$DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix --env PYTHONPATH=/workspace/torch_pnp/alopix:/workspace/torch_pnp/alovb:/workspace/torch_pnp/aloception-oss:/workspace/torch_pnp/alovb/alovb/pnp_transformer nash_pnp`
- when send the log to the W&B, could add the git commit number(add more useful information or description) to make the reproduce easier

#### Git merge
- 经常把main merge到自己的branch（复杂）
- 提出一个merge request -> 详细的描述
- reviewer给出thread -> push commit解决thread，关闭thread
- re-request view

## Windows11
### Make Win11 like Linux
https://zhuanlan.zhihu.com/p/367866550
### Don't use mouse!!! ⌨️
- Windows上 fn+scrlk关闭键盘背光
- Windows上 win+x u u （英文键盘） 关机
- Windows上 powershell中 `New-Item test.txt` 新建文件
- `winget install` powershell安装
- `del`删除文件
- `Rename-Item -Path "qifei.pw1" -NewName ".\qifei.ps1"` 修改文件名

## Ubuntu
常见命令：https://zhuanlan.zhihu.com/p/392986700
### Don't use mouse!!! ⌨️
https://help.ubuntu.com/stable/ubuntu-help/keyboard-nav.html.zh-CN
- close the window -> `alt + F4`
- change the window -> `alt + tab`
- use `ctrl + direction` to move quickly and use `shift` to choose
- zoom in/out -> `ctrl + +/-`
- change the tab/file in vscode -> `ctrl + tab`
- close the file in vscode -> `ctrl + w`
- open more files in vscode -> `ctrl + shift + p + back`
- [more shortcuts in vscode](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-linux.pdf)
- Split terminals horizontally: `Ctrl + Shift + O`
- Split terminals vertically: `Ctrl + Shift + E`
- Scroll in the terminator: `shift + page up/down`
- Move the tab: `Alt + direction'
- how to scroll -> `shift+page up/page down`
- freeze/unfrezze the terminal -> `ctrl+s / ctrl + q`

### set up
- [ ] [zotero](https://www.zotero.org/download/)
- [ ] [flameshot](https://flameshot.org/#download)
- [ ] [vscode](https://code.visualstudio.com/Download)
- [ ] [terminator](https://doc.ubuntu-fr.org/terminator)
- [ ] [zsh](https://blog.imfing.com/2020/06/ubuntu-18-04-theme-terminal-setup/#%E5%AE%89%E8%A3%85-zsh); [my config](https://github.com/GUOkekkk/CodeingTips/blob/main/zsh_config.txt)
- [ ] [git](https://www.digitalocean.com/community/tutorials/how-to-install-git-on-ubuntu-20-04)
- [ ] [docker](https://docs.docker.com/engine/install/ubuntu/)

### Ubuntu 22.04 change the workspace
Go to 'Multitask', using multi-workspace makes the life easier

### count how many files in the current folder
`ls | wc -l`
### record the screen
`ctrl + shift + alt + r`
### ffmpeg
`sudo apt install ffmpeg  `

`ffmpeg -i test.mp4 -vcodec libx264 rotation.mp4`
### sudo nautilus
以root模式GUI打开文件夹
### 脚本语言/Shell
[Bash](https://www.runoob.com/linux/linux-shell.html)就是其中一种，python也属于广义的脚本语言，主要作用就是更好的操作系统

### [Use Terminator](https://www.tecmint.com/terminator-a-linux-terminal-emulator-to-manage-multiple-terminal-windows/#:~:text=Quit%20the%20Terminator%20%E2%80%93%20Ctrl%2BShift,to%20Next%20Tab%20%E2%80%93%20Ctrl%2Bpage_Down)

### [zsh美化终端，但是会有点慢](https://blog.imfing.com/2020/06/ubuntu-18-04-theme-terminal-setup/#%E5%AE%89%E8%A3%85-zsh)

### tmux
[tmux](https://www.ruanyifeng.com/blog/2019/10/tmux.html)分离session 

Modify the prefix 

```
# Set prefix to Ctrl-Space instead of Ctrl-b
unbind C-b
set -g prefix C-Space
bind Space send-prefix
```
but seems the `prefix+d` has the conflict with the terminal, use the `tmux detach` is better.

### history ｜ grep
按条件搜索历史

### draw.io
The best tool I knew since now to draw the flowchart

### 登陆进去黑屏但是cursor可以用
今天以为把公司电脑搞坏了，吓傻了，原来是是google-pinyin和ubuntu20之后的有冲突
```
$sudo apt remove fcitx
$sudo apt remove fcitx-googlepinyin
$sudo apt autoremove
```
### Ubuntu重启
伸出你的左手，同时按住Ctrl+Alt键，别松开
右手先按一下SysRq/PrtSc，左手别松开，等1秒
右手按一下 R，左手别松开，等1秒
右手按一下 E，左手别松开。这时包括桌面在内，所有程序都会终止，你会看到一个黑乎乎的屏幕，稍微等一段时间
右手依次按下 I，S，U，B，左手别松开。每按一次都等那么几秒种，你会发现每按一次，屏幕上信息都会有所变化。最后按下B时，屏幕显示reset，这时你的左手可以松开了，等几秒钟，计算机就会安全重启。

### use Jekyll in local
Jekyll is a static website creation tool.
```
sudo apt-get install ruby-full
sudo gem install bundler
sudo bundle install
```
check the web `bundle exec jekyll serve`
### 在Ubuntu下面修改鼠标侧键
    sudo apt install xbindkeys xautomation
    xbindkeys --defaults > $HOME/.xbindkeysrc
检测侧键

    xev | grep button
    nano ~/.xbindkeysrc
命令

```
#CTRL + C
"xte 'keydown Control_L' 'key c' 'keyup Control_L'"
b:9

#CTRL + V
"xte 'keydown Control_L' 'key v' 'keyup Control_L'"
b:8

#CTRL + TAB
"xte 'keydown Control_L'  'keydown Tab' 'keyup Tab' 'keyup Control_L'"
b:7

#CTRL + SHIFT + TAB
"xte 'keydown Control_L' 'keydown Shift_L' 'keydown Tab' 'keyup Tab' 'keyup Shift_L' 'keyup Control_L'"
b:6
```
The b:2 is already = ctrl+b:1

Need Reboot
### python and python3
Typically the 'python' defaults to 'python3', but in some operation systems, it is not like this. So it is better we use it clearly!
### ln
复制一个链接到另一个地址 ln -s（软复制）用ls查看时有～标志
### mv
移动文件，文件夹/rename

### 删除目录下特定文件名文件
`find . -type f -name "*something*" -delete`

### import bashrc to zshrc
```
vim ~/.zshrc
source ~/.bashrc
source ~/.zshrc

```

### check python env
`which python` or `which python3`

### 清空命令行输入
`ctrl + u`

### check code lines

`wc -l `find . -name '*.py'``

### dvc
[Data Version Control](https://dvc.org/)
### cp
or scp(安全copy) 复制一个文件到另一个文件，需要给要复制的文件的名字
`cp -r` copy the whole folder `mkdir -p todir && cp -r fromdir todir`

#### copy from the server
`scp -r vb-4:`


[a bash shell to copy same file](http://t.csdn.cn/Ua5MO)
### mkdir
### cd
### rm
rm -r 删除整个文件夹

### du -hs *
check the memory

### pwd
输出当前路径

### vi的用法(nano is easier)
https://www.cnblogs.com/emanlee/archive/2011/11/10/2243930.html

Plugin:
- https://www.jiqizhixin.com/articles/2020-06-05-4
- https://zhuanlan.zhihu.com/p/349271041

My `.vimrc`:
```
call plug#begin('~/.vim/bundle')

Plug 'skywind3000/vim-auto-popmenu'

let g:apc_enable_ft = {'*':1}

set cpt=.,k,w,b

set completeopt=menu,menuone,noselect

set shortmess+=c

Plug 'skywind3000/vim-dict'

Plug 'preservim/NERDTree'

Plug 'Yggdroot/LeaderF', { 'do': './install.sh' }

Plug 'jiangmiao/auto-pairs'

Plug 'vim-airline/vim-airline'

Plug 'vim-airline/vim-airline-themes'

Plug 'preservim/nerdcommenter'

let mapleader = ","

call plug#end()
```
#### use '?' to search and 'n' for the next


## VScode
VScode YYDS🏄🏼
### Auto-form does not work
- [ ] check if the settings.json is correct
- [ ] choose the suitable interpreter(with `black` package otherwise `pip install black`)

### [Keyshot in Linux](https://code.visualstudio.com/shortcuts/keyboard-shortcuts-linux.pdf)
The Linux and Windows is different, take care!

`ctrl+G`, find line 

modify the 'go back in navigation locations' to `ctrl + alt + q` 

[some useful shortcuts](https://cult.honeypot.io/reads/20-vs-code-shortcuts-developers/)

### Server error
Error: `error loading webview: error: could not register service worker: invalidstateerror: failed to register a serviceworker: the document is in an invalid state..`

Solution: close all VScode window and run `killall code`

### Pylint to check Python code form
https://blog.csdn.net/jiang_huixin/article/details/125251037

### local history恢复被删除的文件
`ctrl+shift+p`打开command panel搜索`lcoal history entry`

### Debug
https://code.visualstudio.com/docs/editor/debugging

`launch.json` file form:

```
{
    "version": "0.2.0",
    "configurations": [
        {
            "name": "Python: Current File",
            "type": "python",
            "request": "launch",
            "program": "${file}",
            "console": "integratedTerminal",
            "justMyCode": true,
            "args": [
                "--file",
                "/data/vb_office_natural/vb_office_natural.bag",
                "--configuration",
                "NAVDISPARITY-UP0_HS6_ITERS4_LS_OF_BEVFEAT_PI-320-320",
            ]
        }
    ]
}
```
Right click breakpoint -> conidtional breakpoint or log breakpoint

Right click variable & add to watch -> add the variable to the watch window
## Docker用法
https://www.quanxiaoha.com/docker/docker-container.html
### A small example of the docker
docker run --name aloslam_ke(your name)--gpus all -it -v /home/ke/data(your data):/data -v /home/ke/dev/aloslam/aloprodslam(your workspace):/workspace --privileged -e DISPLAY=$DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix aloprodslam:latest(name of the image)

##### Build the image
`sudo -H docker build - < torch_gk_pnp_Dockerfile -t nash_pnp`

##### Build the container
`docker run --name torch-pnp --shm-size=16gb --net=host --gpus all -it -v /data:/data -v /home/ke:/workspace -v /home/ubuntu/weights:/weights --privileged -e DISPLAY=$DISPLAY -v /tmp/.X11-unix:/tmp/.X11-unix --env PYTHONPATH=/workspace/torch_pnp/alopix:/workspace/torch_pnp/alovb:/workspace/torch_pnp/aloception-oss:/workspace/torch_pnp/alovb/alovb/pnp_transformer nash_pnp`

### docker debug
`Cannot connect to the Docker daemon at unix:///var/run/docker.sock. Is the docker daemon running?` -> `sudo systemctl start docker` ( check if docker is running?) -> `Job for docker.service failed because the control process exited with error code. See "systemctl status docker.service" and "journalctl -xeu docker.service" for details.` -> `sudo rm /etc/docker/daemon.json`
##### reboot
reboot or create a new container could solve some wired hardware(nvidia does not initialize) or platform(can not use the xcb) problem
### Can not see the plot in dokcer container
1. when connect to the server `-X`, when run the image `--net=host`
2. add `xhost +` outside the docker

### Enter the container
Not use the `attach`

`sudo docker exec -it cfc30c0330f6 /bin/bash`
## [ChatGPT Prompts](https://writesonic.com/blog/how-to-write-chatgpt-prompts/)

## Git
### Atomic Git Commit
https://sparkbox.com/foundry/atomic_commits_with_git
### Git push时，远端和本地同时修改
先git pull再进行add, commit再git push

### Git修改commit
https://cloud.tencent.com/developer/article/1730774

### git pull does not work

    git fetch --all
    git reset --hard origin/gk_pnp
    git pull

### git clone --recursive
### git checkout
### git log + q
### git branch -a
### Git permission denied
put it on the .bashrc
`eval "$(ssh-agent -s)"
ssh-add ~/.ssh/id_rsa`
and go to `~/.ssh/` do the `sudo chown -R username`

### git delete
```
git checkout master
git branch -d bad_branch
git push origin --delete bad_branch
```

## Markdown语法Tips
### [Emojipeida](https://emojipedia.org/)
### [Cheatsheet](https://www.markdownguide.org/cheat-sheet/)
### md标题没办法引到外部连接
### 生成requirement和项目结构
`pip intsall pipreqs`

`pipreqs .`

`sudo npm install mddir -g`

`mddir` or `mddir /../../`
### 如何添加图片在md文档
1. 比较直接的方法就是把图片上传到repository中然后`![name](link)` 但是容易受DNS域名污染
2. 可以把图片转换到base64码再`![name](data:image/png;base64,XXX)` 但是base64码很长影响写作，可以`![name][base64str]`和`[base64str]:data:image/png;base64,XXX`来代替。`Png2Base64.ipynb`可以用来转换图片到base64码基于python。
Tip：但是不知道为什么我的第二种方法并不成功，第一种方法本地也没办法看到图片，只能用手机才能看到。
3. 或者使用html语言
```
<p align="center">
      <img src="https://img-blog.csdn.net/20151129213701642" width="25%" height="25%" />
      Figure 1. Lena
</p>
```
### 解决看不到自己的readme中的图片
DNS域名污染， 解决办法：
https://segmentfault.com/a/1190000038705840
### 如何打出代码框
使用 `` 反引号 ex：`.md` or `tab` or three `
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
### 偏微分和偏导数
https://www.matongxue.com/madocs/219/
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
 A measure of distance between a point and a distribution.

$$
D(x, Q)^2 = (x - \mu)^T S^{-1} (x - \mu)
$$

Where Q is a probability distribution with mean = u and positive-definite covariance matrix S

### Frobenius norm
It is like the Euclidean Distance for the Matrix

https://mathworld.wolfram.com/FrobeniusNorm.html#:~:text=The%20Frobenius%20norm%2C%20sometimes%20also,considered%20as%20a%20vector%20norm.


### Spherical Harmonics & Spherical Gaussian
都是一种球面基函数，用来表示另一个复杂的非线性函数

Spherical Harmonics：球谐函数， 球面坐标系下的基函数来源于Laplace方程的解，正交，旋转不变性 一阶1一个系数，二阶4个系数，三阶九个系数（常用）

Laplace方程：Laplace算子，二阶偏导和为0, 如果等于一个函数就是Poisson方程（最基础的椭圆方程）

Spherical Gaussian：在球面上服从Gauss分布的基函数，可以自由设计

球面坐标系：可以用颜色也可以用形状来表示一个函数，所以为什么用基函数来表示光照情况，

三维空间下的一种坐标系，就像二维的极坐标系，三维空间常见坐标系：直角坐标系，圆柱坐标系

### KL散度/相对熵
用来衡量两个概率分布的差别的非对称性度量

### [Grobner basis](https://zhuanlan.zhihu.com/p/262906557)
space: https://blog.csdn.net/qq_33458986/article/details/103198580
计算多项式环的理想，高维多元多项式组求解

### SVD
求解最小二乘解或者矩阵求解，求个伪逆。

也是基于特征值分解，结合AtA的特征值分解和AAt的特征值分解，求特征方程

### Pareto front & Nash equilibrium
[Pareto Front](https://en.wikipedia.org/wiki/Pareto_front)

[Nash Equilibrium](https://en.wikipedia.org/wiki/Nash_equilibrium)

[The difference](https://www.quora.com/What-is-the-difference-between-Nash-Equilibrium-and-Pareto-Optimality), example[Prisoner's dilemma](https://en.wikipedia.org/wiki/Prisoner%27s_dilemma)
### 变换
https://zhuanlan.zhihu.com/p/428075759
相机复原：先到affine space再回到Euclidean space

### Normalization & Standardization
- Normalization
scales the values down to the range between 0 and 1

$$ \frac{(x - min(x))}{(max(x) - min(x))} $$

- Standardization
rescales data to have a mean (μ) of 0 and standard deviation (σ) of 1 (unit variance)

$$ \frac{x - u}{\delta} $$


### 有偏估计和无偏估计（方差）
https://kexue.fm/archives/6747

### Convex & Concave
https://learnopencv.com/convex-hull-using-opencv-in-python-and-c/

## 算法知识
最近准备大疆的感知算法工程师感觉还是很多基础知识需要补充学习, 而且很多的中文名字也需要对应一下。
### 四元数 旋转矩阵 旋转向量 欧垃角
`from scipy.spatial.transform import Rotation as R`
#### quaternion
做四元数的时候，注意w的位置在头还是尾，normalization的时候注意维度一致， 一般是norm(q, dim=-1, keepdim=true)
#### rotation matrix
#### rotation vector
#### Euler angle
Normally we choose the `degrees=False`

### Activate function
- Sigmoid

$$ Sigmoid(x) = \frac{1}{1 + e^x} $$

used for the binary classification, easy to cause the vanishing gradient, the gradient of the Relu is small (max=0.25) especially when the |x| is close to 1. After serval small gradients, it is easy to casue the vanishing gradient. Could use the batch_normalization to solve this problem. Make the input of the Sigmoid function is close to the 0.5.

- [Softmax](https://zhuanlan.zhihu.com/p/105722023)

$$ sofxmax(x_i) = \frac{e^{x_i}}{\sum{j=1}{K}e^{z_j}} $$

used for the multi-classification, the key point is the "soft". Compare a hard max, the softmax could give more infomation to the other categories and easy to get the gradient.


- Relu

$$ Relu(x) = max(0, x) $$

compared to the "Sigmoid" or "tanh" (they map the input to the [0,1] or [-1, 1]), during backpropagation, these small gradients are multiplied together, and as the depth of the network increases, the gradients can become exceedingly small.
By enabling larger gradients to be backpropagated, the ReLU activation function allows earlier layers in the network to learn from error signals more effectively, alleviating the vanishing gradient problem to a large extent.
It's worth noting that while ReLU helps with the vanishing gradient problem, it can cause another problem known as the "dying ReLU" problem. This is where a ReLU unit can get stuck during training and always output 0, thereby causing the gradient through that unit to always be 0. Variations of ReLU, such as Leaky ReLU or Parametric ReLU, are designed to mitigate this issue by allowing small negative values when the input is less than 0.

### 梯度消失和爆炸
基本上梯度爆炸是因为权重初始化问题
https://zhuanlan.zhihu.com/p/72589432

### 为什么要做normalization
https://cloud.tencent.com/developer/article/1456997

### pretrain & fine-tuning
https://zhuanlan.zhihu.com/p/389842883

### GRU
https://zhuanlan.zhihu.com/p/394426898

For using the GRU, it is better to choose the `Sigmoid` or the `Tanh` as the activate function(饱和的激活函数)

### VO
#### Feature-based Method
使用feature，然后重投影误差（8点法，5点法。计算快，但是特征计算麻烦。效率低，需要考虑outlier
#### Direct method
计算整个光流， 使用整个图片，但也有semi-direct，用特征周围的区域块。最小化photometic error。

计算耗时间，大的运动很难检测，需要相邻帧变化不大。鲁棒性好，精确，但是对光线变化敏感。

### Outlier Rejection
- [Mahalanobis distance](https://en.wikipedia.org/wiki/Mahalanobis_distance)
- [1-Point RANSAC](https://www.doc.ic.ac.uk/~ajd/Publications/civera_etal_jfr2010.pdf)
- define a ratio to check the distance between the first and second of KNN-BF match
example:
```
        _bf = cv2.BFMatcher(cv2.NORM_HAMMING, crossCheck=False)
        if len(self.previous_des0) == 0 or len(_des1) == 0:
            return None, None

        # Use knnMatch to get the 2 best matches
        _knn_matches = _bf.knnMatch(self.previous_des0, _des1, k=2)

        _good_match = []
        ratio_test = 0.5
        # Ratio test
        assert len(_knn_matches[0]) == 2
        for match1, match2 in _knn_matches:
            if match1.distance < ratio_test * match2.distance:
                _good_match.append(match1)
```
### CNN explainer
https://poloclub.github.io/cnn-explainer/

### 常用矩阵
- 本质矩阵(Essential Matrix) -> 5
- 基本矩阵(Fundamental Matrix) -> 7
- 单应矩阵(Homograph Matrix) -> 8
- 相机矩阵(camera matrix)
https://blog.csdn.net/kokerf/article/details/72191054

### KM algorithm
[增广路定理](https://oi-wiki.org/graph/graph-matching/augment/)
[Hungarian Algorithm](https://zhuanlan.zhihu.com/p/208596378) -> no weights
[Kuhn-Munkres (KM) algorithm](https://zhuanlan.zhihu.com/p/214072424) -> with weights


### [对极约束的问题](https://epsavlc.github.io/2018/11/26/epipolar-geometry.html)

### Levenberg-Marquardt Algorithm
迭代方法，用于非线性最小二乘问题，可以包含非线性参数的问题。通过求解一系列最小二乘问题来逼近最小二乘问题的解。

结合了梯度下降法和Netwon's method。[接近最小值的时候像Netwon下降更快，initial point or deverge考虑更多情况](https://www.cs.cornell.edu/courses/cs4780/2018fa/lectures/lecturenote07.html#:~:text=The%20gradient%20step%20moves%20the,used%20to%20approximate%20the%20function.)。需要计算Jacobian矩阵和LM factor
### Iteratively Rewighted Least Squares
### EndtoEnd learning
不提取数据特征，让模型自己去学习数据。

### 路径规划
#### [RRT(Rapidly-exploring random tree)](https://blog.csdn.net/qq_43310597/article/details/107238684)
[Voronoi diagram](https://en.wikipedia.org/wiki/Voronoi_diagram)
#### PRM(Probabilistic Roadmap)(Dijkstra method)
#### A*
#### [DWA](https://www.guyuehome.com/38209)

### [TCN](https://naokishibuya.medium.com/temporal-convolutional-networks-94293f1a83f8)
### 一些Clustering 方法
- Kmeans
迭代保持中心不变，确定K
- KD tree
本质上二叉树，k维数据分割平面，可以用PCA找节点
-  Hierarchical Kmeans with vocabulary tree
重复使用Kmeans在每个分组中，直到得到最大深度 https://www.jianshu.com/p/6cec9c777853
根据特征对图像进行分类或者聚类便于检索
-  brute-force search
暴力搜索
-  Locality-sensitive hashing
找一个min-hashing map保证变换后的相似性
降低文档相似性比较复杂度https://zhuanlan.zhihu.com/p/108181478
### 相似度计算
- 欧式距离 Euclidean
- 余弦距离/cosine similarity：向量夹角的余弦
- Hamming距离：二元向量的不同
- Jaccard距离：最小的和/最大的和
- 编辑距离：两个字符串经过多少变换可以一致

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

### Zero-shot learning & few-shot learning
http://t.csdn.cn/a4O8C

### Using a fixed conv1D to replace the avg_pool1D could reduce the time
`avg_pool1d(kernel=2, stride=2) = conv1d(kernel=2, stride=2)`

### Variational Autoencoders
https://www.jeremyjordan.me/variational-autoencoders/
### Transformer
https://zhuanlan.zhihu.com/p/48508221

http://jalammar.github.io/illustrated-transformer/

https://www.cvmart.net/community/detail/4032

#### Attention
https://zhuanlan.zhihu.com/p/392553460

#### Key query, value
https://stats.stackexchange.com/questions/421935/what-exactly-are-keys-queries-and-values-in-attention-mechanisms

#### Encoder-decoder
https://easyai.tech/ai-definition/encoder-decoder-seq2seq/

#### [Deep Double Descent](https://openai.com/research/deep-double-descent)

### Regularization
https://0809zheng.github.io/2020/03/03/regularization.html
### Short-cut
From the ResNet, https://www.cnblogs.com/linzzz98/articles/13454369.html
### NLP中的Mask操作
1.为了计算中处理那些补出来的0的信息

2.在decoder中去掉一些文本中的本来的信息，加强训练避免后续分词的影响

### Operator
#### Sobel 一阶微分 过滤模糊的地方
#### Laplace 二阶微分
#### LOG 先Gauss滤波再Laplace算子

### SLAM十四讲
面试笔试的重点，好好复习。 

#### 面试题：
- https://visionary.blog.csdn.net/article/details/115566100?ydreferer=aHR0cHM6Ly9ibG9nLmNzZG4ubmV0L3FxXzM4NTg4ODA2L2FydGljbGUvZGV0YWlscy84ODExOTg5Ng%3D%3D
- https://blog.csdn.net/qq_38588806/article/details/88119896
- https://blog.csdn.net/guanjing_dream/article/details/123787056

#### 笔记
- https://www.cnblogs.com/ivan-chen/p/9496868.html


### ICP
3D和3D来求解T，2dto2d应该也可以，比较困难知道匹配关系.

可以用SVD或者BA来求解
其实ICP在相机坐标系下的点云配准得到的就是相机的pose变换（讨论的时候搞错了）

可以使用Point-to-plane方法，加快收敛速度，避免落入local minimum，使用estimated normal vector上的距离

normal vector可以用当前点和周围邻域的协方差矩阵的最小特征值对应的特征向量求得（PCA）

Using the SVD to get the soulution

Optimize:
- Filter some outlier which is the noise during the data collection
- Use the KDtree structure to save the time

在Open3d里面想得到iPi+1使用`o3d.pipelines.registration.registration_icp(pc3d_i, pc3d_i+1)` 效果不如PnP

### [DLT-PnP](https://zhuanlan.zhihu.com/p/58648937)
利用叉乘来解决Pnp中的尺度不确定性问题（因为尺度不确定不能用最小二乘法）
（PnP应该没有尺度不确定性。。）

### 对极约束
对两张2d图像求解T的方法，通过八对点方法，求解E或者F，存在尺度不确定性

### [三角测量](https://www.zhihu.com/question/27719009)
### PnP问题
已知3D点和对应2d点来求解T，可以用三对点就解决，外加一对点验证.

具体方法有EPnP，DLT等

在opencv里面需要知道相机内参和畸变系数，一种随机方法，非线性最小二乘
得到iPi+1使用`solvePnPRansac(pc3d_i+1, image_i)`

### BA
更多是后段全局优化，最小二乘法收敛光束

### Pose Graph
https://www.youtube.com/watch?v=saVZtgPyyJQ

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

### BERT
Bidirectional Encoder Representation from Transformers，不同于之前的单向Transformer，BERT采用MLM（Marked Language Model）生成双向深度语义特征

### pre-trained network
https://zhuanlan.zhihu.com/p/159620066

PTN or PTM 先通过有标注的较大的通用数据集训练出参数（或者部分参数）负责共性部分，再通过小的针对特殊任务的数据集上的训练，负责特性部分， 可能是zaiPTM的基础上训练或者是只训练输出层

### Bearing Angle Image
基于3D Pointcloud生成的2Dimage基于点和neighbor的关系

### DL+Transdisciplinary
其实我个人对于DL or ML or AI一直以来还很推崇的，计算机的计算性能被最大开发，也越来愈去模仿人脑（所以要读一些脑科学的书）

像孩子学习东西一样构造网络，构造pipeline，像大脑一样对信息进行编码Transformer，我很认可这一定是未来，可能五年之内会有一些决定性的进步（Chatgpt完全不是🙊）

但是现在太多跨学科和DL结合了，控制，感知，生物等等，把一些很优美的公式和算法替代了，变成了不可以解释的AI，也为同行没办法复现出一样的结果找理由。

进行一些换汤不换药的预处理，网络增加几个层，DL里面再加工ML（虽然我本科也是这样😅）。不过只要结果好就是能发论文，而且说不定也真的可以落地，但是也让一些传统算法的发展空间越来越小。不过用DL去做找最优解这个部分我还是很赞成的，本身很多凸优化或者图优化也就是用算力去迭代，和DL区别不大。

`Simplicity is prerequisite for reliability   --Edsger W. Dijkstra`

### EKF
https://simondlevy.academic.wlu.edu/kalman-tutorial/

### [Optical Flow](https://docs.opencv.org/4.1.2/d4/dee/tutorial_optical_flow.html)
https://nanonets.com/blog/optical-flow/

Based on two assumptions:1.The pixel intensities of an object do not change between consecutive frames.
2.Neighbouring pixels have similar motion.
Mainly implemented by using Lucas-Kanade method
- Dense
- Feature
Color represents the direction and the intensity denotes length of displacement vector. It shows the vector information of two continuous frames in one picture

### 常见的Feature（具体看笔记）
https://medium.com/data-breach/introduction-to-orb-oriented-fast-and-rotated-brief-4220e8ec40cf
#### Harris
https://simondlevy.academic.wlu.edu/kalman-tutorial/
#### FAST
#### BRIEF
#### ORB
#### SIFT
#### SURF

### 二叉树遍历
https://blog.csdn.net/My_Jobs/article/details/43451187

### ARP(Address Resolution Protocol)
[ARP attack](https://www.bilibili.com/video/BV1ZW411a7mF/?spm_id_from=333.788.recommend_more_video.-1)

### LIDAR & RADAR
LIDAR: Light; RADAR: ratio/millimeter wave
- 4d lidar(3d positions & velocity)
[example](https://www.aeva.com/aeries-ii/)

### SLAM on ROS Comparison
[RTAB-Map as an Open-Source Lidar and Visual SLAM Library for Large-Scale and Long-Term Online Operation](https://introlab.3it.usherbrooke.ca/mediawiki-introlab/images/7/7a/Labbe18JFR_preprint.pdf)

### Exteroceptive & Proprioceptive
https://www.innowtech.com/2019/09/23/exteroceptive-and-proprioceptive-sensors-for-robotics/#:~:text=Proprioception%20refers%20to%20the%20perception,%2C%20hearing%2C%20etc.).

## 计算机基础
### 解释型语言和编译型语言
https://www.freecodecamp.org/chinese/news/compiled-versus-interpreted-languages/

### pyhon值传递和引用传递
https://cloud.tencent.com/developer/news/709436

在python中也取决于是否变量[可变](https://www.cnblogs.com/blackmatrix/p/5614086.html), so字典还有列表是引用传递

### C++指针传递和引用传递
https://developer.aliyun.com/article/373092

### Assert in Python
https://blog.csdn.net/weixin_39791387/article/details/125187612

### 补码
在计算机系统中，数值一律用补码来表示和存储。原因在于，使用补码，可以将符号位和数值域统一处理；同时，加法和减法也可以统一处理. 正整数的补码是其二进制表示，与原码相同. 求负整数的补码，将其原码除符号位外的所有位取反（0变1，1变0，符号位为1不变）后加1 

【例2】求-5的补码。
-5对应正数5（00000101）→所有位取反（11111010）→加1(11111011)

## 快捷键
记录一些各种各样的快捷键。。。
+ `ctrl+F` 搜索
+ `选中文件+F12` 修改文件名字
+ 在Github页面使用`?`调出键盘快捷键
+ `ctrl+K` word里面插入超链接

## ROS2
https://www.cnblogs.com/shandianchengzi/p/15232145.html
### 如何保存数据--rosbag
Use `rosbag record` to store and `rosbag play` to read.

### Common bug
https://karelics.fi/ros-2-common-issues-and-mistakes/


### check the topic
`rostopic list`

### Insttall packages
update the apt at first `sudo apt update`

then `sudo apt-get install ros-noetic-rviz`



## Python
### PEP 8 Coding Style
https://peps.python.org/pep-0008/ 

- When slicing the array, use the same space before/after the colons, ex: `[0:2:10]` or `[::9]`


### [Python常用运算符](https://www.runoob.com/python/python-operators.html)
简单也是最有效的`0^1=1`; `1^1=0`

`cv2.waitKey(1) == ord("q")`

`1 << n` move to the left n bits, like the x 2^n
`1 >> n` move to the right n bits, like the % 2^n 

`n&1 -> n%2`; `n >>= 1 -> n//2`

### Python Access
https://www.tutorialsteacher.com/python/public-private-protected-modifiers

### Python argparse
https://docs.python.org/zh-cn/3/howto/argparse.html

### Breakpoint()
[breakpoint()](https://www.biye5u.com/article/python/2021/6536.html)

`p variable` -> print; `c` -> next breakpoint; `ctrl c` -> quit

### Assert的用法
https://www.cnblogs.com/sewain/p/14456311.html

### args
`args` is useful for the python development
```
from argparse import ArgumentParser

parser = ArgumentParser(description='test')
parser.add_argument('--input', default=, type=, help = '')
parser.add_argument('--input', default=, action="store_true", help = '')
args = parser.parse_args()
```

### the product of the list
```
from functools import reduce
list1 = [1, 2, 3]
list2 = [3, 2, 4]
 
 # the reduce is used to return a new reduced list
result1 = reduce((lambda x, y: x * y), list1)
result2 = reduce((lambda x, y: x * y), list2)
print(result1)
print(result2)
```
or `np.prod()`

### 阶乘
`reduce(lambda x, y: x*y, [1] + list(range(1, n+1)))`

### 使用glob或者os.listdir来得到文件夹中的文件地址
但是需要注意的是，读取出来的文件是无序的。需要用`list.sort(key = lambda x : int(x.split('something')[0])`
这个sort没有返回值，需要注意
### If `import` does not work
- Check the `echo $PYTHONPATH`
- `export your path` or import the absolute path
### [Pytorch3D](https://pytorch3d.readthedocs.io/en/latest/overview.html)
### tqdm
一个package可以可视化一个迭代器

### ord()
The `ord()` function returns an integer representing the Unicode character.
ex:

    ord('9') - ord('0')

### join
    str.join(sequence)
ex:

    symbol = "-";
    seq = ("a", "b", "c");
    print symbol.join( seq )
    --> a-b-c
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
#### sort and lambda
```
        # sort B based on the value of A[i]
        B = sorted(range(N), key=lambda i: A[i])
```

### String
#### replace
s.replace(" ", "%20")

#### split
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

#### [f-string](https://realpython.com/python-f-strings/)
ex:

      name = "Eric"
      profession = "comedian"
      affiliation = "Monty Python"
      message = (
          f"Hi {name}. "
          f"You are a {profession}. "
          f"You were in {affiliation}."
      )
      message

#### "{}".format
https://www.runoob.com/python/att-string-format.htmlhttps://www.runoob.com/python/att-string-format.html

"""
The {:05d} is a format specification for integer types in Python. It works as follows:

: is the start of the format specification.
0 indicates that the output should be padded with zeros.
5 specifies the width of the output, i.e., the minimum number of characters in the output. If idx is less than 5 digits, it will be left-padded with zeros.
d stands for "decimal", which specifies that the number should be formatted as an integer.
So, if idx is 7, file_name will be "traj_00007.pkl", or if idx is 123, file_name will be "traj_00123.pkl"
"""

### 数位之和
```
def sums(x):
    s = 0
    while x != 0:
        s += x % 10
        x = x // 10
    return s
```
### JSON
Json是JavaScript Object Notation是一种轻量级的数据交换格式.

需要使用`json`这个包来操作。 存在`json.loads`（处理字符串）和`json.load`（处理类文件对象）两种函数。

可以将`json`和`pandas`结合起来使用。https://geek-docs.com/pandas/pandas-read-write/pandas-reading-and-writing-json.html
使用`frame = pd.DataFrame
frame.to_json('.json')`

[JMESPath](https://pypi.org/project/jmespath/)有点像SQL,主要用于搜索

### TensorFlow 2.0
#### 以前的学习笔记
https://github.com/GUOkekkk/TensorFlowLearn
#### TF常用函数

### Numpy
Numpy基本函数 https://cloud.tencent.com/developer/article/1770104
#### Numpy出现维度不对的时候用.ravel把二维变一维
#### [ : : 2]
the form is [start : end : step], so [ : : 2] means form 0 to the end and each 2 steps to take the instance.
#### np.sort
高维数组最好还是用a[np.argsort[:, 1]]
#### 在 np.sort 函数中排序字段
            dt = np.dtype([('name',  'S10'),('age',  int)])
            a = np.array([("raju",21),("anil",25),("ravi",  17),  ("amar",27)], dtype = dt)
            print ('我们的数组是：')
            print (a)
            print ('\n')
            print ('按 name 排序：')
            print (np.sort(a, order =  'name'))
#### np norm axis=i ,remove the i axis on the final result shape
`loss = np.linalg.norm((depths_l[:N] - alo_depth[:N]), ord=1, axis=(1, 2))`

#### np查找满足条件的元素个数
`np.count_nonzero((condition a & conidtion b), axis=0)`
#### np.where()用法
np.where(condition, x, y) 按条件修改数组元素

np.asarray(np.where(condition)).T 返回<nums, n>的符合条件的位置

#### numpy插入一列
np.insert(a, axis, value, axis=1)

#### np.set_printoptions(threshold=1000)
设置打印数据长度

#### 过滤ndarrady中的重复元素
set(tuple([tuple(i) for i in array]))
#### NP数组合并分割
针对一维数组

            np.append(a,b) = np.hstack((a,b))

#### inverse the array
`array[::-1]`

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

### dict/hash table
```
        dic = {}
        for c in s:
            dic[c] = not c in dic
```
`not c in dic` return the bool

After the python 3.6, the dict is ordered based on the insert order

### define a sort rule in Python
```
class Solution:
    def minNumber(self, nums: List[int]) -> str:
        def sort_rule(x, y):
            a, b = x + y, y + x
            if a > b: return 1
            elif a < b: return -1
            else: return 0

        strs = [str(num) for num in nums]
        strs.sort(key = functools.cmp_to_key(sort_rule))
        return ''.join(strs)
```

### all() and any()
any(x)判断x对象是否为空对象，如果都为空、0、false，则返回false，如果不都为空、0、false，则返回true

ex:       ` if any(s < end and start < e for s, e in self.overlaps):
            return False`

note:
+ 不能迭代tuple，只能变成array
+ any 里面的for loop 里面定义的s和e外部没办法调用
+  迭代器里任意一个为真就可以

all(x)如果all(x)参数x对象的所有元素不为0、’’、False或者x为空对象，则返回True，否则返回False

### A better way to get the attribute from the class
```
previous_kp0 = getattr(self, "previous_kp0", None)
```
### Python map
`map(function, iterable)` ex: `nums = list(map(str, nums))`converting every item in the `nums` list to a string
### Opencv
#### cv2只支持unit8<0-255>或者float32<0.0-1.0>
#### [一个方便键盘控制的cv的小demo](https://github.com/GUOkekkk/ToolKit/blob/main/test_OF.py)
#### Opencv不支持SURF
`
pip install opencv-python==3.4.2.16
pip install opencv-contrib-python==3.4.2.16
surf = cv2.xfeatures2d.SURF_create()
`
#### COLOR_GRAY2BGR
Not so sure about this part, but seems the CV2 only could save the color video not the gray

```
    gmap_render = plot_traj(gmap_render, odometry.trajectory)
    # ? why it can only saves the color image?
    gmap_render_rgb = cv2.cvtColor(gmap_render, cv2.COLOR_GRAY2BGR)
    cv2.imshow("gmap_render", gmap_render_rgb)
    if viewhandle is not None:
        viewhandle.write((gmap_render_rgb * 255).astype(np.uint8))  # it needs to be in uint8 format
```

### Python传入和传出的参数最好还是不要_开头
### 内部外部参数也需要注意
### super().__init__(paras)
调用父类的init

### plot大小不一样的子图以及控制坐标轴位置
`plt.figure()` is also based on the  `axes`
- using the variable ax for single a Axes

`fig, ax = plt.subplots()`

- using the variable axs for multiple Axes

`fig, axs = plt.subplots(2, 2)`

- using tuple unpacking for multiple Axes

`fig, (ax1, ax2) = plt.subplots(1, 2)`
`fig, ((ax1, ax2), (ax3, ax4)) = plt.subplots(2, 2)`

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

### Add legends elegantly

    labels_handles = {
        "Estimated cameras": handle_cam[0],
        "GT cameras": handle_cam_gt[0],
    }
    ax.legend(
        labels_handles.values(),
        labels_handles.keys(),
        loc="upper center",
        bbox_to_anchor=(0.5, 0),
    )`
`

### Python Union
TO classify that the input could be multi-type
```
from typing import List, Union

def process_data(x: Union[List[int], int]):
    if isinstance(x, int):
        # If x is an integer, do something
        pass
    elif isinstance(x, list):
        # If x is a list, do something else
        pass
```

### Python Debug mode
```
 # define a function to check the quat is zero or not
def check_zero_quat(quat_data: torch.tensor):
    try:
        assert torch.norm(quat_data) > 1e-3
    except AssertionError:
        print("quaternion has zero quaternion problem after normalization")
        print("quaternion:", quat_data)
        breakpoint()
    return

```

### PyTorch
### [循环生成网络的层](https://zhuanlan.zhihu.com/p/119280719)
ex:

      class Encoder_Block(nn.Module):
          def __init__(self, layers_num = 3, num_hid=128, num_head=8, num_kp = 200, device = 'cuda:0'):
              super(Encoder_Block, self).__init__()
              self.layers_num = layers_num
              self.num_hid = num_hid
              self.num_head = num_head
              self.num_kp = num_kp
              self.device = device
              self.encoder_layers = [] # key tricky

              for i in range(layers_num): # key tricky
                  encoder_layer =nn.TransformerEncoderLayer(d_model=self.num_hid, nhead=self.num_head).to(device=self.device)
                  setattr(self,'encoder_layer%i'%i,encoder_layer)
                  self.encoder_layers.append(encoder_layer)

              self.itmlp = nn.Sequential(
                  nn.Linear(self.num_hid, self.num_hid*2),
                  nn.ReLU(),
                  nn.Linear(self.num_hid*2, self.num_hid//2),
                  nn.ReLU(),
                  nn.Linear(self.num_hid//2, 7),).to(device=self.device)

              self.pnp_check = PnP_check(K=torch.Tensor(np.array([[1,0,0],[0,1,0],[0,0,1]])).cuda(), num_hid=self.num_hid, num_kp=self.num_kp).to(device=self.device)

              self.pos2demb = PositionEmbedding2d(num_hid=self.num_hid, num_kp=self.num_kp).to(device=self.device)

          def __set__init(self,layer):
              init.normal_(layer.weight, mean = 0, std = 1)

          def forward(self, input_emb, pos3d):
              # (B, N+1, num_hid)  (B, N, 3)
              for i in range(self.layers_num): # key tricky
                  output_emb = self.encoder_layers[i](input_emb) # (B, N+1, num_hid)
                  t_token = output_emb[:, -1, :] # (B, 1, num_hid)
                  t_vec = self.itmlp(t_token) # (B, 1, 7)
                  kp2d_check = self.pnp_check(pos3d, t_vec) # (B, N, 2)
                  p2d_check_emb = self.pos2demb(kp2d_check) # (B, N, num_hid)
                  output_emb[:, :-1, :] = output_emb[:, :-1, :] + p2d_check_emb # (B, N, num_hid)
                  input_emb = output_emb
              return input_emb

#### .to(device=device)
make sure or the model/tensor has the smae device
#### .cpu() & .cuda()
numpy only take the .cpu()...but go back to tensor has to use the .cuda()
#### torch.matmul()
好像直接过滤了相同的维度了然后乘法

#### summary
use `from torchinfo import summary` or `from torchsummary import summary` but `torchsummary` is not suitable for the transformer

ex: `summary(model, (3, 640, 128)) # did not take the batch as the input size`

#### .squeeze and .unsqueeze
squeeze压缩tenor，unsqueeze对tensor扩维

#### cat the iterative tensor
ex:

    test = []
    for i in range(10):
      test.append(tensor_i.unsqueeze(0)) # tensor_i (4,4) -> (1, 4, 4)
    torch.cat(test, dim=0) # key tricky

#### torch乘法
torch.einsum!!

dot product: `torch.einsum('bi,bi->b', test1, test2)`

#### Inplace???
error :

    RuntimeError: one of the variables needed for gradient computation has been modified by an inplace operation: [torch.cuda.FloatTensor [1, 200, 2, 64]], which is output 0 of AsStridedBackward0, is at version 2; expected version 1 instead. Hint: the backtrace further above shows the operation that failed to compute its gradient. The variable in question was changed in there or anywhere later. Good luck!

碰到这个问题，首先要找到是哪个tensor有问题（对模型要清楚， 每个tensor的shape都标注出来！）把inplace操作如`x += 1`改成`y = x.clone() y = x+1`

### Python训练加速
https://zhuanlan.zhihu.com/p/389455949
## C++
### size_t
`size_t`是一个无符号整数类型，通常用于表示对象的大小、长度或索引。在C++中，`size_t`是标准库中定义的一个类型别名，它的确切大小和表示取决于平台和编译器，但通常它足够大以表示内存中任何对象的大小。

使用`size_t`的主要原因是：

1. **无符号性**：`size_t`是无符号的，这意味着它只能表示非负整数。这使得它非常适合表示大小、长度或索引，因为这些值通常都是非负的。

2. **可移植性**：由于`size_t`的定义是与平台相关的，所以使用它可以提高代码的可移植性。例如，在32位系统上，`size_t`通常是32位的，而在64位系统上，它可能是64位的。

在上面的代码示例中，`size_t`被用作循环变量`i`的类型，因为`vec.size()`返回的是一个`size_t`类型的值，表示`vector`的长度。使用`size_t`可以确保`i`的范围与`vec.size()`的返回值相匹配，并且避免了可能的类型不匹配警告或错误。

### -> and .
-> 当对象是指针类型时使用

. 当对象是实体

### A good example to filter the data
          if (!std::isnormal(Z_ref) || Z_ref <=0 || Z_ref > slamcf::FE_PNP_MAX_Z_DIST)
          continue;


### ～A()
Destroctor

## JupyterTips
### 使用`esc+f`进入查找替换
### 长按`alt`加移动鼠标多行修改代码
