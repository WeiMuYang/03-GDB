# GDB调试命令      

序号|命令|作用|用法
:-:|:-:|-|-
1|run|启动程序|`run`<br>`r`
2|continue|让中断的程序继续运行|`continue`<br>`c`
3|break|添加断点|`b 函数名`<br>`b 行号`<br>`b 文件名:行号`    #此处是文件名
4|backtrace|调用堆栈|`bt`
5|frame|切换其他堆栈|`f 2`
6|info break|查看所有断点的信息|`info break`<br>`info b`
7|enable<br>disable<br>delete|禁用一个断点<br>启用一个断点<br>删除一个断点|`disable  断点编号`<br>`enable 断点编号`<br>`delete 断点编号`
8|list|查看当前断点处的代码<br>l + 向后显示10行<br>l - 像前显示10行|`l`<br>`l+`<br>`l-`
9|print|输出变量和修改当前内存中的变量值|`print 变量名`<br>`p  变量名`
10|ptype|输出变量的类型|`ptype 变量名`
11 | info breakpoints| 显示所有断点| `info breakpoints`

## 1 常用命令   
1. run命令，简写r，启动程序，Ctrl+C让GDB中断下来   
```shell
run # 简写 r 
```
2. continue命令，简写c，让中断的程序继续运行   
```shell
continue # c
```
3. break命令，简写b ，添加断点  
```shell
b + 函数名  
b + 行号
b + 文件名:行号  # 注意这里是文件名，不是类名    
```
4. backtrace命令，简写bt，查看当前的调用堆栈    
```shell
bt
```
5. frame命令，简写f，切换到其他堆栈处    
```shell
f 2
```
6. info break命令， 查看所有断点的信息   
```shell
info break # 简写 info b
```

7. enable命令、disable命令、delete命令    
```shell
disable + 断点编号 # 禁用某一个断点
enable + 断点编号  # 启用某一个断点
delete + 断点编号  # 删除某一个断点
```
8. list命令，简写 l，查看当前断点处的代码， l + 向后显示10行， l - 像前显示10行   
```shell
l
l+  
l-
```
9. print命令，简写p， 输出变量和修改当前内存中的变量值   
```shell
p + 变量名
```
10. ptype命令，输出变量的类型    
```shell
ptype + 变量名
```

## 3 参考资料   
1. https://www.cnblogs.com/--lr/p/11189609.html     
2. https://www.cnblogs.com/--lr/p/11189609.html   