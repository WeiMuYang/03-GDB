# GDB查看STL库中对象的值     

[toc]

## 概述  
在进行GDB调试过程，发现vector和list里面的值，不能查看里面的值，这样对开发带来很大的不便。 因此，在网上查看相关的资料，用来打印Vector和List里面的值。  

## 配置文件   
1. 进入链接：http://www.yolinux.com/TUTORIALS/src/dbinit_stl_views-1.03.txt      [本地位置](../10-others)

2. 全选里面的内容，并把内容复制到dbinit_stl_views-1.03.txt文本文件中   

3. 通过命令将文本文件的内容，复制到~.gdbinit中   

```shell
   cat dbinit_stl_views-1.03.txt >> ~/.gdbinit
```

4. 进入GDB中，运行命令：

```shell
source ~/.gdbinit
```

## GDB调试   
省略   

## 参考资料   

1. https://blog.csdn.net/hit0803107/article/details/84196659   
2. https://blog.csdn.net/nancygreen/article/details/17789677?utm_medium=distribute.pc_relevant_t0.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-1.vipsorttest&depth_1-utm_source=distribute.pc_relevant_t0.none-task-blog-2%7Edefault%7EBlogCommendFromMachineLearnPai2%7Edefault-1.vipsorttest   