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

整形

```c
#include <stdio.h>
int main()
{
    int a=5,b,c,d,e,f;
    b=a+2; # b=5+2=7
    c=b-a; # c=7-5=2
    d=a*c; # d=5×2=10
    e=a/d; # e=5/10=0.2=0 , 抹掉小数位0
    f=a%d; # f=5%10=5 , 取余数
    return 0;
}
```

小数\(浮点\)

```c
#include <stdio.h>
int main()
{
    double a,b,c,s;
    a=3.67;
    b=5.43;
    c=6.21;
    s=(a+b+c)/2;
    return 0;
}
```

字符

```c
#include <stdio.h>
int main()
{
    # 大写字母A加1为B
    # 大写字母A加2为C
    # 大写字母加32位其小写字母,减去同理
    char a='B',b='O',c='Y';
    a=a+32; #a='b';
    b=b+32; #b='o';
    c=c+32; #c='y';
    # 上面还可以写成这样
    a+=32;
    b+=32;
    c+=32;
    x*=(y+8); # x = x*(y+8);
    z%=3; # z = z%3;
    return 0;
}
```

**用printf语句输出int , float , double , char型数据**

**int**

\n - 换行

%d - 整数替代

printf - 后面的变量依次替换

```c
#include <stdio.h>
int main()
{
    int a=5,b,c,d,e,f;
    b=a+2; # b=5+2=7
    c=b-a; # c=7-5=2
    d=a*c; # d=5×2=10
    e=a/d; # e=5/10=0.2=0 , 抹掉小数位0
    f=a%d; # f=5%10=5 , 取余数
    printf("a=%d,b=%d,c=%cd\n",a,b,c);
    printf("e=%d,f=%d",e,f);
    return 0;
}
```

求整数123与456的和.

```c
#include <stdio.h>
int main()
{
    int a,b,sum;
    a=123;
    b=456;
    sum=a+b;
    printf("和等于%d\n",sum);
    return 0;
}
```

**double**

%f - 小数替代

```c
#include <stdio.h>
int main()
{
    double a,b,c,s;
    a=3.67;
    b=5.43;
    c=6.21;
    s=(a+b+c)/2;
    printf("设定的a是%f,b是%f,c是%f\n",a,b,c);
    printf("求得的s是%f\n",s);
    return 0;
}
```

**char**

%c - 字符替代

```c
#include <stdio.h>
int main()
{
    char a='B',b='O',c='Y';
    a=a+32; #a='b';
    b=b+32; #b='o';
    c=c+32; #c='y';
    printf("小写字母依次是%c%c%c\n",a,b,c);
    return 0;
}
```

练习

给"orya"加密 , 加密规律是 : 用原来字母后面的第一个字母代替原来字母.

```c
#include <stdio.h>
int main()
{
    char c1,c2,c3,c4;
    c1='o';
    c2='r';
    c3='y';
    c4='a';
    c1+=1;
    c2+=1;
    c3+=1;
    c4+=1;
    printf("加密后的英文是:%c%c%c%c\n",c1,c2,c3,c4);
    return 0;
}
```

**用scanf语句输入int , float , double , char型数据**

int型

```c
#include <stdio.h>
int main()
{
    int a,b,s;
    scanf("%d|%d",&a,&b);
    s=(a+b)/2;
    printf("%d与%d的平均是%d\n",a,b,s);
    return 0;
}
```

float

```c
float a,b;
scanf("%f,%f",&a,&b);
```

double

```c
double a,b;
scanf("%lf,%lf",&a,&b);
```

char

```c
char a,b;
scanf("%c,%c",&a,&b);
```

编写一个程序 , 输入大写字母 , 可以输出小写字母

```c
#include <stdio.h>
int main()
{
    char a;
    printf("请输入大写字母:\n");
    scanf("%c",&a);
    b=a+32;
    printf("%c的小写字母是%c\n",a,b);
    return 0;
}
```

**putchar\(\)语句和getchar\(\)语句**

putchar输出字符

getchar输入字符

```c
#include <stdio.h>
int main()
{
    char a,b,c;
    a=getchar();
    b=getchar();
    c=getchar();
    a+=32;
    b+=32;
    c+=32;
    putchar(a);
    putchar(b);
    putchar(c);
    putchar('\n');
    return 0;
}
```



