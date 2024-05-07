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
直接在想要转换类型的变量前加上要转换成的类型的类型名称
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
#### 2.2.2 while语句


## 3.函数
### 3.1 声明函数
Todo

### 3.2 调用函数
Todo

### 3.3 递归函数
Todo

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
