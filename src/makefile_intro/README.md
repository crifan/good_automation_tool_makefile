# Makefile简介

## 什么是`Make`和`Makefile`

* `make`是一个`脚本工具`=`script tool`，一般（尤其是`Linux`类的系统中）也叫做`命令`=`command`
  * 并且`Linux`类系统中的一般都已经内置安装了`make`
* `Makefile`是一个`文本文件`，一般也叫做`脚本`=`script`
  * 是自己，根据`make`的语法，写的，用于各种要做的事情，实现对应的功能
* `用法`：当你输入了`make`命令后，`make`会去根据你写的`Makefile`中的规则去执行对应的动作
  * 最典型的用途是，Linux系统中用`make`根据`*.c`去编译生成`*.o`目标文件

## `Makefile`的用途和用法

类似于`Makefile`的工具，主要用于实现：

* 将：低效率的，需要手动的多个步骤输入多个命令，才能完成的工作
* 变成：每次只需要，高效率的，运行`make`命令去完成各种复杂的功能
  * 当前，前提是，需要先写好对应的`Makefile`文件

即所谓的`自动化脚本`

目的是：`提高工作效率`

本人之前最早接触Makefile，是在嵌入式开发期间，有很多的系统、工具、软件，都需要利用makefile去编译、配置。

比如：Linux内核的make menuconfig后再去make编译

后来在移动互联网开发期间遇到makefile，更多的是：

将各种繁琐的人工要敲不同命令才能实现的功能，用makefile去实现一键搞定的效果

## `Makefile`和其他自动化工具的区别

而自动化脚本，其他也有很多工具和软件可以实现，比如Linux中的`shell`等。而Makefile和shell等不同之处和侧重点是：主要根据文件依赖关系，主要用于文件编译。

而实际上可以利用文件依赖关系，去实现更广泛的、做事情的先后顺序有依赖关系，也可用`Makefile`去实现

比如自己的[Crifan的Gitbook的模板](https://github.com/crifan/gitbook_template)中的[Makefile](https://github.com/crifan/gitbook_template/blob/master/GitbookCommon.mk)，就是用`makefile`脚本是实现：

* 本地调试gitbook
* 编译出不同格式的文件
* 发布到服务器上

等等功能，其中内部利用了不同的步骤的先后依赖关系，实现自动化的效果的。

> #### Note:: 详见帖子
> [【已解决】提取Gitbook中Makefile公共部分](http://www.crifan.com/gitbook_extract_common_part_of_makefile)
