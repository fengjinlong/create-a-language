写在源文件中的源代码是人类可读的源。它需要"编译"，转为机器语言，这样 CPU 可以按给定指令执行程序。C 语言编译器用于把源代码编译成最终的可执行程序。这里假设您已经对编程语言编译器有基本的了解了。

(一).安装

1.为了在 Windows 上安装 GCC，需要到MinGW 的主页 www.mingw.org，进入 MinGW 下载页面，下载最新版本的 MinGW 安装程序。或者到：http://sourceforge.net/projects/mingw/files/，下载 Download mingw-get-setup.exe (86.5 kB)

2.运行 Download mingw-get-setup.exe ,点击"运行"，continue等，注意记住安装的目录，如 D:\MinGw,下面修改环境变量时还会用到。

3.修改环境变量:

 选择计算机—属性---高级系统设置---环境变量，在系统变量中找到 Path 变量，在后面加入 min-gw的安装目录，如 D:\MinGw\bin
4.在开始菜单中，点击"运行"，输入 cmd,打开命令行:输入 mingw-get,如果弹出 MinGw installation manager 窗口，说明安装正常。此时，关闭 MinGw installation manager 窗口，否则接下来的步骤会报错

5.在cmd中输入命令 mingw-get install gcc,等待一会，gcc 就安装成功了。

如果想安装 g++,gdb,只要输入命令 mingw-get install g++ 和 mingw-get install gdb

(二)使用

在桌面创建一个hello.c的程序


hello.c
在 cmd 中输入命令 gcc C:\Users\12057\Desktop\c语言\helloworld\hello.c


image.png
在当前目录下(记住是命令的当前目录)会生成 a.exe 的可执行文件，在 cmd 中输入 a.exe 就可以执行程序了。
hello world

https://www.jianshu.com/p/dc0fc5d8c900