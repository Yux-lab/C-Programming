## 11.1　指针变量
在用指针变量p存储变量i 的地址时，我们说p “指向”i;
指针就是**地址**，而指针变量就是存储地址的变量
![[Pointers.png]]

当谈论变量 `i` 的地址时，通常指的是这个变量的“基地址”或“起始地址”，即存储这个变量的第一个字节的地址。
![[1.png]]


### 指针变量的声明
```C
//指向int 类型 对象(变量) 的指针变量
//初始化
int *p;
```

## 11.2 取地址运算符和间接寻址运算符
& :(取地址)运算符
如果x是变量，那么&x 就是x 在内存中的地址。

```c
int i, *p;
//把i的地址赋值给变量p
p = &i
```
![[2.png]]

### 11.2.2 间接寻址运算符
* (间接寻址)运算符访问存储在对象中的内容。
```c
//显示i的值
//对*p 的改变也会改变i的值,它们是共存亡的
printf("%d\n", *p);

//逆运算
j = *&i;  /* same as j = i; */
```

## 11.3 指针赋值
```c
int i, j, *p, *q;

//把i的地址复制给p
p = &i;

//p的内容（即i的地址）复制给q
q = p;
```

![[3.png]]
