# vscode_project_maker
## 概述
工作n年了，工作环境一直是台式机，所以整了个双硬盘分别装了windows和linux，平时的开发就在linux下，普通工作就在windows下，虽然经常切换系统感觉比较麻烦，但是凑合下也就算了。不过，在2019年12月，爱折腾的我终于给自己换了一个工作。新公司给我配了一台装好了win10专业版的笔记本，这家伙，就像刘姥姥进大观园，头一遭啊！怎么安装linux？怎么安装开发环境？没办法，经过两个月的折腾，终于使用win10+hyper-v+vscode整合出了一个开发环境，该方法在win10中开启HYPER-V，然后安装CentOS和Ubuntu虚拟机，最后安装vscode，这一切完成后，使用该工程提供的脚本初始化虚拟机，创建C/C++，GO,PYTHON,JAVA工程供主机上的vscode开发。
接下来从**安装**，**新建工程**，**编译调试工程**这三个角度来进行说明。

# 安装
## 开启hyper-v
要开启并使用hyper-v，需要满足以下三个条件：

1 操作系统是windows 10专业版(据说windows 10家庭版也可以，但是未进行测试)。

2 CPU支持intel硬件虚拟化技术。

3 可以连接互联网。


对于满足该条件的机器：

第一步，重启机器，进入BIOS，开启intel硬件虚拟化支持。具体的开启方法根据BIOS厂商而异，请自行百度。

第二步，下载vscode_project_maker(https://github.com/boboniu2004/vscode_project_maker)，并且解压缩。

第三步，进入vscode_project_maker\\.ssh目录，选中**inithyper-v.bat**脚本，单击右键以管理员权限运行，如果执行权限不对或者不是windows10专业版，脚本会报错。

第四步，如果正确开启了hyper-v，则会要求重启，重新启动后进入vscode_project_maker\\.ssh目录，以管理员权限再次运行**inithyper-v.bat**脚本，会创建虚拟网卡共后续的虚拟机进行通信。

**至此hyper-v开启完毕。**


## 安装linux虚拟机
## 安装vscode

# 新建工程

# 编译调试工程
