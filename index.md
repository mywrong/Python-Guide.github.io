# python简介
## 1 python是什么
python是一门新手友好的计算机编程语言，就像人与人之间的交流需要使用汉语、英语等许多门语言，人与计算机的交流也有很多语言，python就是其中一门人和计算机都可以理解的语言。总的来说，我们按照python的语法规则，写下某些有特定意义的语句，计算机就可以理解我们的意图，并帮助我们实现想要的功能。

## 2 为什么要学习python
1、就像汉语英语日语一样，有的语言学起来容易，有的语言学起来困难，python在所有计算机编程语言中是最容易学习的语言之一，如果不是专门作为开发工具，只是作为一种提升工作效率的工具或者用来实现一些实用的功能的话，python是一门很好的入门语言。

2、python现成的库（别人写好的已经实现了某些功能的代码）很多，语言生态非常好，学一两个月就可以写出一些有实用价值的程序了，这种学习中的正反馈，对于初学者十分重要，而python能很快提供这种正反馈。

## 3 python可以用来做什么
对于财务工作者：自动化操作excel，可以减少枯燥的重复劳动，可以使用数据透视表快速进行分类汇总，自由组合字段快速计算。

对于产品经理、数据分析师：使用python爬虫可以自动化的从目标网站获得你想要的数据。

对于学生、科研工作者：python丰富的可视化图表库可以让你的论文图表丰富多彩，脱颖而出。

# 安装python编程环境
在安装python编程环境前首先需要了解以下几个概念：

## 1 什么是编程环境？
编程环境主要包含python解释器(Interpreter)与python库。

### 1.1 什么是python解释器
计算机只能执行二进制的机器语言，因此需要python解释器将我们从键盘输入的python代码翻译成计算机能够理解的机器语言，在windows系统python解释器通常是名为python.exe的文件。

### 1.2 什么是python库
想象一下我们正在造一把小铁锤，可能需要用到一些工具，比如锯子，车床，我们不可能为了造铁锤而再去造把锯子，造台车床，最好的办法就是去把别人造好的锯子和车床买来直接用。python库就是我们在造铁锤中可能会用到的锯子和车床。本着开源精神，一些程序员在使用python解决了一类问题后，为了避免其他人在这类问题上重复花费精力，他们将自己编写的代码公开在网络上供所有人使用。有了python库我们可以更快速的实现想要的功能。

## 2 学习python需要安装的软件
对于初学者，推荐使用anaconda+pycharm这两款软件。不同操作系统的安装方式有所不同，本文如无特别说明都以win10为例。
### 2.1 anaconda
我们在编写不同的代码来实现各种功能时，不可避免的会使用不同版本的python解释器或者各种python库。假如我为了实现A功能已经安装了python 2.7版本的解释器，现在我又想实现B功能，但是我发现B功能只能使用python 3.6版本的解释器,那么我们该怎么办？

anaconda就是解决这一矛盾的软件。如果把计算机系统看作一个大口袋，为了解决python版本以及可能存在的python库冲突，anaconda把每种编程环境放进一个小口袋，小口袋间相互隔离，再将小口袋放入大口袋，这样就解决了编程环境冲突的问题，其中小口袋我们称之为虚拟环境。
#### 2.1.1 安装anaconda
anaconda官网：https://www.anaconda.com/

下载页面：https://www.anaconda.com/products/individual#Downloads

![avatar](https://github.com/mywrong/Python-Guide/blob/master/image/anaconda/anaconda%E4%B8%8B%E8%BD%BD%E9%A1%B5%E9%9D%A2.png?raw=true)


使用windows 64位操作系统的同学可以选择64-Bit Graphical Installer (477 MB)进行下载。

下载完成后点击.exe文件进行安装，安装路径可以选择任意目录，但是注意路径不能包含中文，然后全部直接next即可。

#### 2.1.2 配置环境变量

1.

![anaconda配置环境变量1](https://github.com/mywrong/Python-Guide/blob/master/image/anaconda/anaconda%E9%85%8D%E7%BD%AE%E7%8E%AF%E5%A2%83%E5%8F%98%E9%87%8F1.png?raw=true)

2.

![anaconda配置环境变量2](https://github.com/mywrong/Python-Guide/blob/master/image/anaconda/anaconda%E9%85%8D%E7%BD%AE%E7%8E%AF%E5%A2%83%E5%8F%98%E9%87%8F2.png?raw=true)

3.

![anaconda配置环境变量3](https://github.com/mywrong/Python-Guide/blob/master/image/anaconda/anaconda%E9%85%8D%E7%BD%AE%E7%8E%AF%E5%A2%83%E5%8F%98%E9%87%8F3.png?raw=true)

4.

![anaconda配置环境变量4](https://github.com/mywrong/Python-Guide/blob/master/image/anaconda/anaconda%E9%85%8D%E7%BD%AE%E7%8E%AF%E5%A2%83%E5%8F%98%E9%87%8F4.png?raw=true)

5.

![anaconda配置环境变量5](https://github.com/mywrong/Python-Guide/blob/master/image/anaconda/anaconda%E9%85%8D%E7%BD%AE%E7%8E%AF%E5%A2%83%E5%8F%98%E9%87%8F5.png?raw=true)
其中"D:\environment\Anaconda3"是我anaconda的安装路径，替换成自己anaconda的安装路径即可。

#### 2.1.3 创建虚拟环境

1. win+r打开运行窗口，输入cmd，打开命令行窗口。在命令行窗口输入`conda`，按下enter键，如出现以下结果则说明anaconda环境配置成功。conda是anaconda中用来创建和管理虚拟环境的主要工具，使用conda我们可以仅使用一个命令就可以下载网络上其他程序员贡献的开源Python库。

2. conda换源。如前所述，conda会根据我们输入的命令，自动的去某个网站下载我们想要的python库，conda默认的下载网址是国外的网站，在国内下载速度较慢，因此推荐将conda的默认下载网址换成国内的网站。

    在命令行窗口输入一下三行命令。
    ```
    conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
    conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/conda-forge
    conda config --add channels https://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/msys2/
    conda config --set show_channel_urls yes
    ```
    这样我们就完成了conda换源。

3. 现在我们可以使用conda来创建自己的虚拟环境了。在命令行窗口输入`conda create -n environment_name python=X.X`，其中`environment_name`是你要创建的虚拟环境的名称，建议根据创建此环境的目的来命名，比如我们的目的是学习python，就可以将`environment_name`替换为`python-learning`，当然，命名风格因人而异。`X.X`是我们要使用的python解释器版本，比如`2.7`、`3.6`、`3.7`、`3.8`、`3.9`，也可以不写`pyhton=X.X`，此时默认使用anaconda的默认python版本。

    我们这里创建一个名为`python-learning`的虚拟环境，输入命令`conda create -n python-learning python=3.7`，按下enter键，若出现`CondaHTTPError:HTTP 000 CONNECTION FAILED`字样的提示，这是网络连接出现了错误，解决办法如下：

    具体步骤如下所示：

    打开`C:\Users\Pot`目录，其中`Pot`需要替换为本机windows系统账户名，在这个目录下有一个名为`.condarc`的隐藏文件
    ![conda创建虚拟环境报错1](https://github.com/mywrong/Python-Guide/blob/master/image/anaconda/conda%E5%88%9B%E5%BB%BA%E8%99%9A%E6%8B%9F%E7%8E%AF%E5%A2%83%E6%8A%A5%E9%94%991.png?raw=true)

    使用记事本作为打开方式打开`.condarc`，将其中替换为以下内容
    ```
    channels:
      - http://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/msys2/
      - http://mirrors.tuna.tsinghua.edu.cn/anaconda/cloud/conda-forge/
      - http://mirrors.tuna.tsinghua.edu.cn/anaconda/pkgs/free/
    show_channel_urls: true
    ```

    保存并关闭文件，再重新输入`conda create -n python-learning python=3.7`，按下enter键，出现一下提示，我们再输入y，表示确定创建此虚拟环境，最后等待conda帮我们创建虚拟环境就可以了，如下图所示。
    ![conda创建虚拟环境](https://github.com/mywrong/Python-Guide/blob/master/image/anaconda/conda%E5%88%9B%E5%BB%BA%E8%99%9A%E6%8B%9F%E7%8E%AF%E5%A2%83.png?raw=true)
    
    这里询问我们是否要继续创建虚拟环境，我们输入y表示确认。

    conda自动下载完一些必须的库后就完成了虚拟环境的创建。
    ![conda创建虚拟环境2](https://github.com/mywrong/Python-Guide/blob/master/image/anaconda/conda%E5%88%9B%E5%BB%BA%E8%99%9A%E6%8B%9F%E7%8E%AF%E5%A2%832.png?raw=true)









