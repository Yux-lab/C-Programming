

### 2.1.1 编译和链接
预处理(执行以#开头的命令(指令))→编译(将程序翻译成机器指令(目标代码))→链接(将目标代码和附加代码(比如库函数printf)整合)

GCC/IDE(软件包，可在其编辑、编译、链接、执行以及调试)

### 2.2.1 指令
pun.c
```
#一般形式
指令

int main(void)
{
    语句
}


#include <stdio.h> 指令 头文件
#为什么要使用头文件？因为C语言的输入/输出功能是由标准库的函数实现的

#int表明函数返回一个整数值；void表明函数没有参数
int main(void)
{
    printf("To C, or not to C:that is the question.\n");

    #使函数终止；其次指出返回值为0
    return 0;
    
}
```

## 2.3 注释
```
/*  */

C99新注释
// 
```

## 2.4变量和赋值
### 2.4.1 类型
int,float

### 2.4.2 声明
使用变量前：先声明，后赋值
```
int height;
float profit;

#合并声明
int height, length, wideth, volume;
```
### 2.4.3 赋值
```
int height = 8;

#包含小数点的常量赋值给float变量时，后面加一个字母f
float profit = 2150.48f;
```

### 2.4.4 显示变量的值
```
printf("Height: %d\n", height)
#占位符'%d'(仅用于int型变量),指明值要放在哪个位置显示

printf("profit: $%.2f\n", profit)
#占位符'%.2f'用于显示float型变量。默认显示小数点后6位。
#如若强制显示小数点后p位，则把'.p'放在%和f中间。
```
