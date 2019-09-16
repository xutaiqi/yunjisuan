# 云服务计算作业第三周

搭建 Golang开发环境
  
    使用的Ubuntu虚拟机，所以虚拟机上进行环境的安装
    首先在网站 https://studygolang.com/dl 上下载golang的安装包，
    之后在安装包的目录下在终端调用指令：sudo tar -zxvf go1.13.linux-amd64.tar.gz 来解压安装包
   ![](https://github.com/xutaiqi/yunjisuan/blob/master/imag/4.png)
      
      之后要配置环境变量
      运行指令 sudo vim /etc/profile
    在文件最后一行加入：
    export GOROOT=/home/xutaiqi/go
    export GOPATH=/home/xutaiqi/Work/go
    export GOBIN=$GOPATH/bin
    export PATH=$PATH:$GOROOT/bin
    export PATH=$PATH:$GOPATH/bin
    之后，保存退出
    然后调用指令：source /etc/profile 来使配置生效。
   ![](https://github.com/xutaiqi/yunjisuan/blob/master/imag/1.png)
    
    之后安装git工具
    调用指令 sudo apt-get install git
    安装完成后，调用指令 git version
   ![](https://github.com/xutaiqi/yunjisuan/blob/master/imag/2.png)
    
    安装VS ，在网站下载安装
    
编写第一个package
    
      之后创建包路径：
      mkdir -p $GOPATH/src/github.com/user
      之后在该目录下创建go文件
      编写 hello.go 文件
   ![](https://github.com/xutaiqi/yunjisuan/blob/master/imag/3.png)
   
      然后创建一个库
      mkdir $GOPATH/src/github.com/user/stringutil
      编写reverse.go文件
   ![](https://github.com/xutaiqi/yunjisuan/blob/master/imag/5.png)
      
      之后编写reverse_test.go文件作为测试文件      
   ![](https://github.com/xutaiqi/yunjisuan/blob/master/imag/6.png)
  之后开始运行文件
    ![](https://github.com/xutaiqi/yunjisuan/blob/master/imag/7.png)
    ![](https://github.com/xutaiqi/yunjisuan/blob/master/imag/8.png)
