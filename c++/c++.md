## day1
#### 与C语言的的区别
引入了<font color=red>命名空间</font>的概念
输出方式不同，<font color=red>cout</font>是一个<font color=red>流对象</font> 不同于printf库函数
C语言中的左移运算符 << 在C++中是<font color=red>输出流运算符</font>

#### 命名空间
背景: 在两个公司进行合作时，很大概率发生命名的冲突(变量名相同, 函数名相同, 或者struct相同)

C语言解决方法: 对于所有变量或者函数在命名时会加上公司信息 
如 google 和 facebook
int google_num=1； int facebook_num=2
C++解决方法: 使用命名空间
namespace google{
  int num; int register();
}

#### 命名空间的使用
```
// :: 指作用域限定符
// 命名空间中定义的变量 函数  对象 都称为命名空间的一个实体

namespace::func();

例如
namespace wd{
int num=1;
void display(){cout<<"nihao";}
}
wd::display  // 访问wd中的display函数
```
#### 常量
用于记录程序中不可更改的数据
- #define宏常量    
     语法:  #define 变量名 值
      通常在文件上方定义 表示一个常量
- const修饰的变量 
  语法: const 数据类型 变量名= 常量值
  通常在变量定义前加关键字 必须初始化
```
#define day 7
const int week=7
```

####数据类型
#####字符串型
- C风格字符串 char 变量名[] =" 字符串值"
- C++风格字符串 string 变量名 ="字符串值"
- 
```
char str[]="hello,world"
string str="hello world"
```
#####布尔类型bool
true 真  false 假  
bool类型占1个字节

#####数据的输入
cin>> 变量

####运算符
#####递增递减

++a 和 a++
前置递增 先让变量+1 然后进行表达式的运算
后置递增 先进行表达式的运算，后让变量加1
```
int a =10；

int b1=++a*10      先加1再乘10  110
int b2=a++*10      先乘10再加1  101

```

逻辑运算符
|运算符|术语|示例|结果|
|---|---|---|---|
|!|非|!a|a为假 则!a为真|
|&&|与|a&&b|a,b都为真 为真
||或|a||b|a,b有一个为真则为真|

三目运算符
表达式1 ? 表达式2 :表达式3
表达式1为真 执行表达式2 否则执行表达式3 








