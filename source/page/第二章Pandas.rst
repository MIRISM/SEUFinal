.. final term documentation master file, created by
   sphinx-quickstart on Wed Jun  3 23:09:49 2020.
   You can adapt this file completely to your liking, but it should at least
   contain the root `toctree` directive.




第二章 pandas
==================================

在成功利用Tushare获取股票信息后，这章我们来学习如何利用pandas进行数据分析，首先我们这样安装及导入模块::

 pip install pandas
 import pandas as pd
 
pandas的两个核心数据结构为Series和Dataframe。DataFrame是一个表型的数据结构，它含有一组有序的列，每列间可以是不同的数据类型（数值，字符串，布尔值等）。DataFrame既有行索引又有列索引，其中的数据是以一个或多个二维块存放的，而不是列表，字典或别的一维数据结构。虽然它是个二维的结构，但是DataFrame任然可以表示更高维的数据（利用层次化索引的表结构）。

由于tushare返回数据均为Dataframe形式，本章节只对Dataframe的操作进行介绍。