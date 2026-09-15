# C语言知识第二讲表达式和选择语句

* 1.if else条件

当没有括号时如：

```
if(a==5)
  printf("a");
else
  printf(a);
```

只能包含一个语句，剩下语句无效。

或者包含括号，可以使用、多个语句

```
if(a==5)
   {
    printf("a");
    a*5;
   }
  else
   {
     printf(a);
    }
    return 0;
```

else悬空

else会跟最近的if联立，当出现多个if时

如：

```
if(num!=8)
    if(num!=5)
    else
  num*5+1;
    printf("%d",num);
return 0;
```

这里说明第一个if包含所有条件，如果正确则跳过下面所有ifelse循环，直接进行输出。

2.布尔值（BOOL）

仅含有两种取值，真或假，对应1或0，在C99标准中，引入了\_Bool类型，这是一个内置的布尔类型，它的值只能是0或1。非0的值在赋给\_Bool变量时会被转换为1。C99还提供了\<stdbool.h>头文件，定义了bool代表\_Bool，true代表1，false代表0。

bool后面跟的数可以是负数，代表0.

* 2.表达式

1.语句和表达式

2.算术运算符

1. 一元运算符： + -表示数字的正负
2. 二元运算符：+、-、\*、%、/ 表示两个数以上进行计算。（%不能为浮点数，只能为整数计算）

3.复合赋值

-=、/=、\*=、%=

分别代表对数减赋值，余赋值，乘赋值，取余赋值。

4.自增运算符

i++=i+1=++i

但++i在switch里不常见，也不普及，容易与+=混淆。

* switch（字符）；

\{

case（条件）；

…

default（否则） ;

}

如：

```
switch (grade) {
  case "A"；
    printf("很棒！\n");
break;
  case "B"；
  case "C"；
    printf("做得好\n");
break;
  case "D"；
    printf("您通过了\n");
break;
  case "F"；
    printf("最好再试一下\n");
break;
default；
  printf("无效的成绩\n");
}
  printf("您的成绩是 %c\n", grade);
return 0;
}
```

​
