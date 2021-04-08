# DDD的安装与配置   

## 1 DDD的安装   

```shell
sudo apt install ddd
```

## 2 DDD的配置  
### 2.1 字体设置  
- 原始的ddd字体丑陋，像素化，需要设置合适的字体大小，点击Edit->Preferences->Fonts。然后看到不同设置。然后点击Browse   
- 点击图中的fmly,选择fixed(这是系统提示作者选fixed的，本人ubuntu系统，不同系统可能不同)，然后点击ptSz，选择字体大小，我选的200，然后点击select保存即可。其他Browse都是类似设置。最后点击OK保存即可。     

### 2.2 显示行号   
- 行号是十分重要的信息，在调试时十分有用，可是默认没有显示，需要自己设置。点击Edit->Preferences->Source，然后选中Display Source Line Numbers即可。    

### 2.3 图形化显示数据   
ddd是一个借助与gdb的强大的图形化debug工具。它可以使得gdb是可视化的，不再是枯燥的命令行的形式。而且它支持数据的显示，包括列表和图的形式等。特别是图的形式，在进行debug时特别直观而有用。    

### 2.4 gnuplot 的设置   
由于ddd使用gnuplot画图，所以确认系统上安装了gnuplot,未安装的话则sudo apt-get install gnuplot即可。打开Edit->Preferences->Helpers可以看到Plot设置的选项，Plot Window选项为External或者Builtin。我选择的是External，不知道为何，选中Builtin时在画图时一直是显示Starting gnuplot的状态。这样就设置好了gnuplot。    


## 3 参考资料  
1. https://www.jianshu.com/p/5d521d0cf633     
2. https://www.cnblogs.com/spinsoft/archive/2012/07/09/2582089.html   