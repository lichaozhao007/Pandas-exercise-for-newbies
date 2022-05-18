 
# 数据分析入门


## A.如何在线快速部署环境并运行本教程？
提供以下两种方式：
1. 通过binder引擎，自己配置
 - 进入[mybinder](https://mybinder.org) 
 - 在github repo栏，输入本github地址即可：https://github.com/lichaozhao007/Pandas-Exercises/ 
 - 点击launch，等待浏览器加载，就弹出一个新tab，可在线运行本教材的jupyter notebook 
![image](https://user-images.githubusercontent.com/62827484/168116706-ebe5c877-e8cc-4799-acbb-6cc88842cb86.png)

2. 直接进入我已配置的编辑环境
[**我的binder**](https://mybinder.org/v2/gh/lichaozhao007/Pandas-Exercises/HEAD)




### B.本地运行如何操作？
**本地运行**
工欲善其事必先利其器，如果想利用python进行数据分析，那么git clone下载到本地，并在自己的系统上**运行jupyter notebook（推荐通过conda安装）**，掌握这些工具就是最好的入门，当然也不用一上来就下载pycharm这样的重型开发工具。

+ **1）查看python版本
- 先查看是否安装了python 3.7以上版本 ：

`
 $ python -V
`

- 接着Git Clone到本地

`
 $ git clone https://github.com/adamli-86/Pandas-Exercises.git
`

+ **2）运行notebook**

` 
 $ jupyter notebook 
`

+ **3）浏览器会自动打开notebook，主页就是文件目录，找到该文件夹即可**
 
 
 
### 如何使用conda，并安装jupyter？

**安装三件套**
> anaconda（或miniconda） + Jupyter Notebook 

**方法如下**
1. **确保已经安装python(或conda）和panda库**
```
$ python -V
$  pip install pandas
```
如果显示版本号说明已经系统已经安装过或本身自带paython（original的版本号），这种情况建议安装

2. **下载Jupyter**
如果没有任何显示，说明没有python，建议Anaconda（**一次性安装python和常用数据分析包**），想解约空间或只是玩玩数据分析，也可以miniconda（_只有python和依赖包，后续可以通过conda安装其他高级的数据分析package_）
```
 $ pip install conda
 or
 $ conda install python
``` 
若显示base的版本号（不是系统自带的original的版本号），证明系统已经成功安装conda（及附带的python），若显示original的版本号，请重新安装

3. **安装jupyter notebook**

```
- $ conda install jupyter notebook
- $ conda run jupyter notebook
(或者直接：$ jupyter notebook）
```

**Conda的基本命令**

1.基本操作：
- 升级全部库：  conda upgrade --all
- 升级一个包  conda update packagename
- 安装包：conda install packagename
-也可以安装多个包：   
conda installl numpy pandas scipy
-安装固定版本的包：conda install numpy =1.10
-移除一个包：conda remove packagename 
-查看所有包：conda list 

2.管理python环境：
-创建虚拟环境：conda create -n env_name list of packagenaem
eg:  conda create -n env_name pandas 
- 指定python版本：conda create -n env_name python2 = 2.7 pandas 
- 激活环境： activate env_name
- 退出环境 :  deactivate  env_name
- 删除虚拟环境：conda env remove -n env_name
+ 显示所有虚拟环境：conda env list  

- **名词和背景解释**
- Pandas：Python的数据处理库，可以进行数据探索、处理数据和输出基本报表（dataflame格式）。
- python：主流的开发语言之一，可以跨平台使用的编程语言，尤其适合网络开发和数据分析（包括机器及深度学习），是万能的胶水语言。
- conda：一种通用包管理系统，旨在构建和管理任何语言和任何类型的软件。
- jupyter notebook：数据分析的轻便但强大的编辑器，可以在浏览器上打开网页直接运行，敲代码直接enter就出结果，也能装各种插件。
- pycharm：python流行的编辑器之一，不限于数据分析。
 

 


