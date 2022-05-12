
 
# 数据分析入门

利用Python的*数据处理库pandas*，可以进行数据探索、处理数据和输出基本报表（dataflame格式）。 

- **快速运行**
可直接在线的jupyter服务器运行本练习:
[binder服务器](https://mybinder.org/v2/gh/lichaozhao007/Pandas-Exercises/HEAD)

- **本地运行**
工欲善其事必先利其器，如果想利用python进行数据分析，那么git clone下载到本地，并在自己的系统上**运行jupyter notebook（推荐通过conda安装）**，掌握这些工具就是最好的入门，当然也不用一上来就下载pycharm这样的重型开发工具。

- **名词和背景解释**

- python是万能的胶水语言，尤其擅长网络开发和数据分析。

- conda是一种通用包管理系统，旨在构建和管理任何语言和任何类型的软件。

- jupyter notebook是数据分析的轻便但强大的编辑器，可以在浏览器上打开网页直接运行，敲代码直接enter就出结果，也能装各种插件。
 
- pycharm是python流行的编辑器之一，不限于数据分析。
 
### 操作步骤 

+ **1）下载本教材
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
 $ conda run jupyter notebook 
`

+ **3）浏览器会自动打开notebook，主页就是文件目录，找到该文件夹即可**
 
 
 
### 如何使用conda，并安装jupyter？

**三件套**
```
 Python(pandas) + anaconda（或miniconda） + Jupyter Notebook 
```
**方法如下**
1.**确保已经安装python(或conda）和panda库**
```
$ python -V
$ conda -V (可选)
$  pip install pandas`
```
如果显示版本号说明已经系统已经安装过或本身自带paython（original的版本号），这种情况建议安装

**在conda下载Jupyter**
如果没有任何显示，说明没有python，建议Anaconda（**一次性安装python和常用数据分析包**），想解约空间或只是玩玩数据分析，也可以miniconda（_只有python和依赖包，后续可以通过conda安装其他高级的数据分析package_）
```
 $ pip install conda
 $ conda install python
``` 
若显示base的版本号（不是系统自带的original的版本号），证明系统已经成功安装conda（及附带的python），若显示original的版本号，请重新安装

2.**确保安装了jupyter notebook**

`
$ conda run jupyter notebook
`

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


 


