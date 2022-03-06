
 
## 菜鸟数据分析入门 （Python Data Analysis）

 
 
**首先，工欲善其事必先利其器，安装你的数据分析工具是最好的入门。**

在conda环境运行Jupyter，利用Python的强大的库pandas，可以进行数据探索和建立数据报表。 


 
 
### 操作步骤 

* **1）Git Clone下载到本地电脑**

`
 $ git clone https://github.com/adamli-86/Pandas-Exercises.git
`

* **2）运行notebook**

` 
 $ conda run jupyter notebook 
`

* **3）浏览器会自动打开notebook，主页就是文件目录，找到该文件夹即可**
 
### 前提 
***Python(pandas、seaborn) + conda环境 + Jupyte rNotebook*** 
+ **1.确保已经安装conda、python**
```
 $ conda -V

 $ python -V
``` 
如果显示版本号说明已经系统已经安装过或本身自带paython（original的版本号），这种情况建议安装miniconda作为补充。

如果没有任何显示，说明没有python，建议Anaconda（一次性安装python和**常用的package，尤其是数据分析的**。
```
 $ pip install conda

 $ conda install python
``` 
若显示base的版本号（不是系统自带的original的版本号），证明系统已经成功安装conda（及附带的python），若显示original的版本号，请重新安装

+ **2.确保安装了jupyter notebook**

`
$ conda run jupyter notebook
`

**也可以通过Jupyter Notebook官方安装：


官方说明： https://jupyter.readthedocs.io/en/latest/install.html 


