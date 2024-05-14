# Python For Algorithm

历史：诞生于上世纪80年代末，比Java（1995.05）、JavaScript(1995.11)差不多早5年，比C++（1985）差不多晚五年。2000年后，Python才成为全球最流行的十大编程语言之一,2018后Python稳居流行度排名首位。

哲学：优美、直白、简洁、易懂、易读

## 0.开始
可在在线平台运行python程序：<https://www.online-python.com/>

1、用python打印hello world

```python
print('hello world')
````

2、用python做计算

```python
1 + 1
3.14 * 2
````

## 1.变量

### 1.1 给它一个名字
例子1:
```python
message = 'hellow world'
print(message)
```

例子2:
```python
a = 1
a + a
```

例子3:
```python
pi = 3.14
r = 2
pi * r
```

**_注意：想看结果可以用print打印出来_**  

例子4:
```python
pi = 3.14
r = 2
result = pi * r
print(result)
```

例子5:
```python
a = 1
b = 2
result = a < b
print(result)
```


### 1.2 值的类型
几种常见的类型：int（整数）, float(浮点数), str(字符串), bool(布尔值)  
int: 3  
float: 3.14  
str: 'hello world'  
bool: True  

### 1.3 计算
int: 整数可以+(加)、-(减)、*(乘)、//(整除)、%(取余)  
```python
1 + 1
2 - 1
3 * 5
6 // 2
5 // 3
6 % 2
5 % 3
```

float: 整数可以+(加)、-(减)、*(乘)、/(除)  
```python
1.0 + 1.0
2.0 - 1.0
3.0 * 5.0
6.0 / 2.0
5.0 / 3.0
```
python作为弱类型语言，可以在不同数字类型之间做运算，返回其中更高精度的数字类型。

特别地，两个整数之间做除法的时候会返回浮点数，不论是否更够整除。

**_注意：想看结果可以用print打印出来_**  

bool：布尔值可以or(或)、and（且）、not（非）  
```python
1 == 1 or 1 != 1
1 == 1 and 1 != 1
not 1 == 1
not 1 != 1
```


str:字符串可以使用'+'进行连接   
```python
firstName = 'zhang'
lastName = 'san'
fullName = firstName + lastName
print(fullName)
```
  
类型转换： 
有时候，我们需要对数据内置的类型进行转换，数据类型的转换，一般情况下你只需要将数据类型作为函数名即可。
Python 数据类型转换可以分为两种：
 (1)隐式类型转换 - 自动完成
 (2)显式类型转换 - 需要使用类型函数来转换
在隐式类型转换中，Python 会自动将一种数据类型转换为另一种数据类型，不需要我们去干预。
在显式类型转换中，用户将对象的数据类型转换为所需的数据类型。 我们使用 int()、float()、str() 等预定义函数来执行显式类型转换。
```python
piValue = float('3.14')
piName = str(3.14)
luckyNumber = int('12')
```


## 2.控制

### 2.1 条件执行语句
条件即选择，如果满足某一条件，就进行某一操作，不满足则不进行。
python中有三种常用条件执行语句

if
```python
if 1 == 1:
    print(true)
```
if else
```python
if 1 == 1:
    print(true)
else:
    print(false)
```
if elif else
```python
if 1 == 1:
    printf(1 == 1)
elif 1 == 2:
    print(1 == 2)
else:
    print(1 == 3)
```
**_注意：想看结果输出可以使用print打印出来_** 

### 2.2 循环执行
当我们需要将某一操作连续执行多次时，可以使用循环语句让代码在我们所设定的条件内反复执行，当不满足循环条件时，便会退出循环继续执行之后的代码
#### 2.2.1 for语句
for循环直接在range(start, stop[, step]),  中括号里面表示可选参数,  start:起始值。  stop:结束值(不包括stop本身)  step:隔step打印一次。
具体示例看下面
```python
for i in range(0, 10):
    print(i)

# 或者创建一个列表，将结果先存储在列表中，最后打印列表即可:
lst = []
for j in range(0, 10, 2):
    lst.append(j)
print(lst)
```

#### 2.2.2 while语句
while 判断条件(condition)：
    执行语句(statements)……
```
# 具体示例：
count = 0
while (count < 9):
   print('The count is:', count)
   count = count + 1
 
print ("Good bye!")
```

## 3.函数
函数是组织好的，可重复使用的，用来实现单一，或相关联功能的代码段。
### 3.1 声明函数
以 def 关键词开头，后接函数标识符名称和圆括号()。
任何传入参数和自变量必须放在圆括号中间。圆括号之间可以用于定义参数。
函数内容以冒号起始，并且缩进。
return [表达式] 结束函数，选择性地返回一个值给调用方。不带表达式的return相当于返回 None。
```python
def printme( str ):
   "打印传入的字符串到标准显示设备上"
   print(str)
   return
```

### 3.2 调用函数
定义一个函数只给了函数一个名称，指定了函数里包含的参数，和代码块结构。
这个函数的基本结构完成以后，你可以通过另一个函数调用执行，也可以直接从Python提示符执行。
下面的例子就调用了printme()函数
```python
# 定义函数
def printme( str ):
   "打印任何传入的字符串"
   print(str)
   return
 
# 调用函数
printme("我要调用用户自定义函数!")
printme("再次调用同一函数")
```

### 3.3 递归函数

```
# 例子，算个5的阶乘：

def recursion(n):
  if n == 0 or n == 1:
    return 1
  else:
    return n * recursion(n - 1)
s = recursion(5)
print(s)

'''
递归：就像朋友之间拉扯，先从外向内传递出去，然后再从内向外（按照某种运算）依次收回来。
以上recursion(5)，函数定义的内部计算细节过程如下：
===> recursion(5)
===> 5 * recursion(4)
===> 5 * (4 * recursion(3))
===> 5 * (4 * (3 * recursion(2)))
===> 5 * (4 * (3 * (2 * recursion(1))))
===> 5 * (4 * (3 * (2 * 1)))
===> 5 * (4 * (3 * 2))
===> 5 * (4 * 6)
===> 5 * 24
===> 120

'''


```
### 3.4 作用域
Todo

### 3.5 Typing
Todo


## 4.List & Tuple
### 4.1 List基础用法
Todo

### 4.2 使用循环遍历List
Todo

### 4.3 List切片
Todo


## 5.String
Todo


## 6.Set & Map
Todo
