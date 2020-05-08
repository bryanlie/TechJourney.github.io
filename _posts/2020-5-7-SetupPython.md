---
layout: post
comments: true
title: How to install Python
---

## 如何安装Python

# 什么是Python

Python 是一种高级编程语言，它是一种动态的面向对象的脚本语言。

1. Python的用途
它是一种通用的语言，主要应用于数据处理，人工智能，web应用开发等领域。

2. Python的优缺点

优点： 简单易学，语法简洁，强大丰富的库，开发效率高等

缺点： 执行速度慢，难于多线程编程等

# 安装 Python

1. 直接装 Python3

<https://www.python.org/downloads/>

2. 安装 Anaconda
如果安装Anaconda，不需要先安装Python，强烈推荐使用。Anaconda是Python包管理器，且集成了环境管理的功能。如果觉得Anaconda太大，可以考虑安装miniconda。

<https://www.anaconda.com/products/individual> 

3. Pip
另一个Python包管理器，安装Python的时候已经自动安装。如果要管理环境，需要另外安装Virtualenv。

# 开发环境

1. 编辑器, 比如 notepad, gedit

2. Jupiter Notebook
是基于网页的交互式计算应用程序，可应用于开发、文档编写、运行代码和展示结果。

使用Anaconda安装

```
conda install jupyter notebook
```

使用pip命令安装， 先把pip升级到最新版本

```
pip install --upgrade pip
pip install jupyter
```

运行，直接在终端中输入以下命令：
```
jupyter notebook
```

3. IDE, 比如PyCharm

<https://www.jetbrains.com/pycharm/download/>

# 实践
```
print('Hello, World!')
```
