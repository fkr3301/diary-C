# C语言知识第三讲-循环语句的结构

* 1.while条件语句

while（条件）

\{

执行语句

}

如：

显示5到1

```c
int i=5；
while(i)
{
  printf("%d",i);
  i=i--;
}
return 0;
```

2.do语句

do（语句）

\{

​

}

最后执行再进行判断

3.for循环语句

for(表达式；表达式；表达式)

\{

​

​

}

while和for循环的区别

主要在于选择和进行，while是挑取条件进行循环，for循环是固定次数循环，循环维护性更高。

如：

```c
for(i=5;i>0;i--)
{


}
```

与

```c
while(i>0)
{
  i=i--;
}
```

表达相同，for更简洁。

for可以省略表达

在C99中for条件里可以直接定值

如：

```c
for(int i=5;i>0;i--)
{


}
```

4.逗号运算符

用于在条件中分开，用于添加条件

素数代码（素数（质数）：只有自己和一的因素的数）

```c
#include(stdio.h)
int main()
{
printf("请输入一个素数")；
sacnf("%d",&num);
for(i=2;i<num;i++)
{
num%i==0;
break;
}
if(i<num)
{
printf("这个数不是素数")；
}
else
{
printf("这个数是素数")；
}
```

1. continue语句

跳转到循环末尾，循环继续执行

go to语句

如

```c
int num;
scanf("%d",&num);

goto(num);
{
a;
printf("A");
b;
printf("B");
c;
printf("C");
}
```

则会通过输入的进行条件读取。

​
