# 快速总结

#### 基本语法

**固定格式**

```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    return 0;
}
```

**printf语句**

```c
#include <stdio.h>

int main() {
    printf("Hello, World!\n");
    printf("你好,世界!\n");
    return 0;
}
```

> \n - 换行 . \t - 空格

练习

```c
#include <stdio.h>

int main() {
    printf("*******\n");
    printf("你好,宝贝\n");
    printf("*******\n");
    return 0;
}
```

**int , float , double , char数据**

变量赋值 : 要先定义这个变量

```c
int a=3;
float b=3.14; # 允许的小数点后面的位数相对少一点,省空间
double c=3.14; # 允许的小数点后面的位数相对多一点,相对占空间
char d='hi';

# 赋多个值(3种写法一样)
int a=1,b,c=3; # 定义a是个整数1,b是个整数,c是个整数3
-----
int b;
int a=1;
int c=3;
---
int a,b,c;
a=1;
c=5;
```



