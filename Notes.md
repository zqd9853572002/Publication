# Week 1 - 2

## 资源

- [总站](www.py4e.com)

### 参考书

[参考书 - Python for Everybody: Exploring Data In Python 3](https://www.py4e.com/book)

- [在线版1](https://www.py4e.com/html3/)，[在线版2](https://books.trinket.io/pfe/index.html)
- [中文版-在线](https://github.com/RodenLuo/py4e-cn/tree/master/book3)

### 视频

- [中文版翻译 - b站](https://www.bilibili.com/video/av46649799)

### 课件和code

- [课件和code](https://www.py4e.com/materials)
  - [课件](https://www.py4e.com/lectures3/)
  - [code打包下载](https://www.py4e.com/code3.zip)

## 练习题

- [PY4E练习题(需登录)](https://www.py4e.com/assignments)

### 在线python编辑器

- [python code playground - coursera](https://www.coursera.org/learn/python/ungradedLti/LqMCR/python-code-playground-developing-python-in-the-browser)

- [Trinket](http://trinket.io/)
- [Cloud9](http://c9.io/)
- [CodeAnywhere](https://codeanywhere.com/)

# Week 3 -  Writing Paragraphs of Code

- python中的结构

  |                         | 举例           | 对应书的章节 |
  | ----------------------- | -------------- | ------------ |
  | variable, reserved word | 字             | 2            |
  | valid syntax pattern    | 句             | 3-5          |
  | construct program       | 段落和整篇文章 |              |

## 字和词

- reserved word是对python有特殊意义的词，不能在其他地方使用reserved word（即reserved word有且仅有一个含义）
- 只要有reserved word出现，python就会认为其有特殊意义
- reserved word包括
  - and, del, global, not, with, as, elif, if, or, yield, assert, else, import, pass, break, except, in, raise, class, finally, is, return, continue, for, lambda, try, def, from, nonlocal, while

## 句子

- 每行代码都是一个句子，句子组成段落
  - 句子必须使用正确的syntax
- sentence包括variable，operator，constant，function等

## 篇章

- 不要在交互环境中放入过多行的代码，要将代码放入script文件中(*.py)
  - python会逐行读取script中的代码

### 构成程序的积木

- program中，有的步骤sequential step（按顺序执行），有的步骤属于conditional（执行时会跳过），有的步骤属于可重复，有的步骤用于存储数据

  - sequential step：按顺序执行即可。在代码中显示是没有缩进

    ![](https://s3.ax1x.com/2020/12/01/Df1DWF.jpg)

  - conditional step，用于条件判断，显示为缩进

    ![](https://s3.ax1x.com/2020/12/01/Df1Wo6.jpg)

  - repeated step: 让程序一直循环，直到满足一定条件后，才跳过循环。显示为有缩进

    ![](https://s3.ax1x.com/2020/12/01/Df1xfS.jpg)

    - loop中必须有检查项，改变项（iteration variable）

# Week 4 -  Expression

## 参考书目

[中文版](https://github.com/RodenLuo/py4e-cn/blob/master/book3/02-variables.mkd)

[英文版](https://books.trinket.io/pfe/02-variables.html)

## 上课笔记

### constant

- constant value不会变
- constant的分类
  - numeric constant
    - 整型：没有小数点的数字
    - 浮点型：有小数点的数字
  - string constant

### reserved word

- reserved word包括
  - and, del, from, None, True, as, elif, global, nonlocal, try, assert, else, if,, not, while, break, except, import, or, with, class, False, in, pass, yield, continue, finally,  is, raise, def, for, lambda, return
  - 不能使用保留词命名

### variable

- 可对variable进行赋值

  - assignment statement是将值赋给变量（先进行等号右边的运算，将运算完的结果赋给左边的变量）

    ```python
    x = 3.9 * x * (1-x)
    ```

- variable的命名
  - 必须由字母或下划线开始
  - 可包括字母，数字，下划线
  - 区分大小写（一般都用小写）
- variable取名时，需要取便于理解的名字 

### numeric expression

- operator: + - * / **(指数) %（取余数）

  - / 会产生float（带小数点），即真正的除法

    ```python
    >>> 30 / 5		#不管此处是不是int，/的结果都是float
    6.0
    ```

- operator的计算顺序

  - 括号 > 指数 > * / % > + - 
  - 从左到右运行

- data type对于operator各不相同

  ```python
  >>> asd = 1 + 4
  >>> print (asd)
  5
  >>> asd = 'he' + 'is'
  >>> print (asd)
  heis
  
  # 不能用str +/- int/ float，没有意义
  >>> asd = 'a' + 1		
  Traceback (most recent call last):
    File "<pyshell#18>", line 1, in <module>
      asd = 'a' + 1
  TypeError: can only concatenate str (not "int") to str
  ```

- 可使用type()获取data的type

  ```python
  >>> type ('see')
  <class 'str'>
  >>> type (1)
  <class 'int'>
  >>> type (304.1)
  <class 'float'>
  
  ```

### 错误的解释

```python
>>> see = 'see' + 1
Traceback (most recent call last):						# 告知发生错误
  File "<pyshell#9>", line 1, in <module>				# 告知错误在哪
    see = 'see' + 1
TypeError: can only concatenate str (not "int") to str	#告知是什么错误
```

### 数据类型的转换

- 可使用函数转换数据类型

  - int(), float(), str()

    ```python
    >>> int ('500')
    500
    >>> float(3)
    3.0
    >>> str (30)
    '30'
    
    # 如果用int()转换float，则会舍弃小数部分，向下取整
    >>> int(98.6)
    98
    
    # 如果数值中没有数字，则int/ float函数会报错
    >>> int ('ce')						
    Traceback (most recent call last):
      File "<pyshell#17>", line 1, in <module>
        int ('ce')
    ValueError: invalid literal for int() with base 10: 'ce'
    ```

### input()

- input()是让用户输入值，所有输入的值都会自动转成str（字符串）

  ```python
  # 此处不管输入什么类型的值，都会转成str
  >>> name = input ('your name: ')
  your name: 123		
  >>> name
  '123'		# 不管输入什么类型的值，input()都会转成str
  ```

### comment

- #之后可以加入注释（注释会被程序忽视掉，不会执行）
- comment的作用
  - 描述接下来的code的作用
  - 说明是谁写的代码
  - 暂时disable一行代码

### 案例

#### 问题

- 让用户输入楼层，转换floor层数

#### 思路

- 输入
  - 用input()获得用户的输入
- 处理
  - 转换层数
- 输出
  - 用print()输出结果

#### 解答

```python
# 转换输入的楼层数

# 输入
inp = input ('Europe floor? ')	# 程序在此处暂停，用户输入的值都是str

# 处理
us_floor = int (inp) + 1		# 此处不能忘了要用int()把用户的输入值转换为整数

# 输出
print ('US floor is', us_floor)	# ,会产生一个空格
```

## 测试题

### 习题 2



### 习题 3

```python
'''
编写一个程序，提示用户输入工时和时薪，然后计算出总工资。

Enter Hours: 35
Enter Rate: 2.75
Pay: 96.25

我们暂时不用担心我们计算的结果是否能正好精确到小数点后两位。如果你非常想的话，可以试一试Python内置的 round 函数，它可以把结果约到两位数。
'''

hour = input ('input your hours: ')
rate = input ('input your rate/ hour: ')
pay = float (hour) * float (rate)
print ('your pay is ', round (pay, 2))
```

# Week 5 - Conditional Code

## 参考书目

[中文版](https://github.com/RodenLuo/py4e-cn/blob/master/book3/03-conditional.mkd)

[英文版](https://books.trinket.io/pfe/03-conditional.html)

## 笔记

### 执行条件

- 各种比较不会改变variable本身的值

#### comparison oeprator

|      | 意思                       | mark     |
| ---- | -------------------------- | -------- |
| <    | 小于                       |          |
| <=   | 小于等于                   |          |
| ==   | 等于（判断两个值是否相等） | 两个等号 |
| !=   | 不等于                     |          |
| >=   | 大于等于                   |          |
| >    | 大于                       |          |



#### 布尔表达式

- 可以表示True/ False

- 使用==来比较运算对象

  ```python
  # 使用==来比较运算对象, 两者相等则返回True，否则返回False
  # =用于赋值，==用于比较
  
  >>> 5 == 5
  True
  >>> 5 == 6
  False
  
  # True和False属于布尔类型
  >>> type(True)
  <class 'bool'>
  >>> type(False)
  <class 'bool'>
  ```

- 比较运算符

  ```python
  x != y
  x > y
  x < y
  x >= y
  x <= y
  x is y
  x is not y
  ```

#### 逻辑运算符

- and/ or/ not

  |      | 解释                         |
  | ---- | ---------------------------- |
  | and  | 两者都为True时，才为True     |
  | or   | 只要有一个值为True，即为True |
  | not  | 取反                         |

- 所有非0的数字都是True

  ```python
  # 所有非0的数字都是True
  >>> 123.01 and True
  True
  ```

### 执行各种条件

- 条件语句可以检查条件，并据此改变程序的执行顺序

  ![](https://s3.ax1x.com/2020/12/02/D4w1r6.jpg)

- 如果判断条件为真，则执行方块中的内容

  ![](https://s3.ax1x.com/2020/12/02/D4Br4g.jpg)

- 缩进（indenting）部分可能会执行，也可能不执行。但程序会执行所有未缩进的部分

  - 正确的缩进非常重要，决定了python是否能正确执行程序
  - tab和4个空格不一样（即使看上去可能一样），此处需要非常注意

#### if

- if语句步骤

  ![](https://www.py4e.com/images/if.svg)

- if语句

  ```python
  '''
  if之后跟条件
  条件之后要加:
  具体要执行的步骤要缩进
  '''
  
  if x > 0:
      print('x is positive')	# 如果条件为真，则执行此步
  ```

  ```python
  # if语句中要执行的步骤也可以不缩进
  if x > 0: print('x is positive')
  ```

- 案例 (nested decision，嵌套语句)

  ![](https://s3.ax1x.com/2020/12/02/D4BI5F.jpg)

- 如果尚未决定条件为真时的步骤，则可使用pass跳过

  ```python
  # 使用pass跳过条件为真时的步骤
  
  if x < 0:
      pass
  ```

#### else (two-way decision)

- if + else是只有2种可能性的情况。条件会决定执行if之后的内容还是else之后的内容(但只执行其中一项，不会两个都执行)

- 案例1

  ![](https://s3.ax1x.com/2020/12/02/D4BLK1.jpg)
  
- 案例2

  ```python
  if x%2 == 0:
      print('x是偶数')
  else:
      print('x是奇数')
  ```

  ![](https://www.py4e.com/images/if-else.svg)

  - else属于分支

#### elif

- elif适用于有2+种可能性的情况（elif是else if的缩写），即连续判断

- elif只能执行if代码块中，各种可能性中的一种，之后直接结束

  ![](https://s3.ax1x.com/2020/12/02/D4rrlj.jpg)

- 执行完x < 2之后，直接跳过if代码块中的其他代码，直接进入结果

  ![](https://s3.ax1x.com/2020/12/02/D4rWkT.jpg)

- elif的步骤

  ![](https://www.py4e.com/images/elif.svg)

- elif只执行某一个分支，之后直接结束if代码块

  ```python
  if choice == 'a':
      print('Bad')
  elif choice == 'b':
      print('Good')
  elif choice == 'c':
      print('Maybe')
  ```

  ```python
  if x < 2:
      print ('below 2')
  elif x >= 2:
      print ('greater or eaqual to 2')
  else:
      print ('something else')	#不管x取什么值，这步都不会被执行，因为x已经满足了上述条件，且执行完if中的一个条件或elif后，直接结束代码块
  ```
  
  
  
- 会按顺序执行，如果第一个条件是false，则检查下一个条件，如果还是false，则继续检查下个条件，直到检查到一个true的条件（也有可能没有true，此时直接结束if代码块）

#### 嵌套条件语句

- 可在一个if中，嵌套另一个if

- 嵌套语句步骤

  ![Nested If Statements](https://www.py4e.com/images/nested.svg)

  ```python
  if x == y:
      print('x等于y')
  else:
  
      # 嵌套条件语句，再次加入逻辑判断
      if x < y:		
          print('x小于y')
      else:
          print('x大于y')
          
  # 代码可以优化为
  if x > 0 and x < 10:
      print ('x在0-10的范围内')
  ```


### 使用try和except找异常

- 代码运行过程中可能会出错，可使用try-except来避免出错

  - 方式为在可能出错的代码前加入try，说明可能有错，但不让python报错
  - 在可能出错的代码后加except，说明如果try中代码出错，则执行except中的程序

- try-except运行方式

  - 如果try中的代码工作正常，则跳过except中的代码

  - 如果try中的代码工作异常，则执行except中的代码

    ![](https://s3.ax1x.com/2020/12/02/D4snjs.jpg)

- 可使用try和except排除异常

  ```python
  # 换算摄氏度和华氏度
  inp = input('Enter F Temperature: ')
  fahr = float(inp)
  cel = (fahr - 32.0) * 5.0 / 9.0
  print(cel)
  
  # 如果客户输入数字，则没问题
  Enter F Temperature: 4
  -15.555555555555555
  
  # 如果客户输入文字，则会报错
  Enter F Temperature:  test
  Traceback (most recent call last):
    File "/tmp/sessions/e9e3759dde07dd1d/main.py", line 2, in <module>
      fahr = float(inp)
  ValueError: could not convert string to float: 'test'
  ```

  ```python
  # 此时可在可能要出问题的语句前加try和except，用以避免错误
  
  inp = input('Enter F Temperature:')
  
  '''
  此时加入try: 之后的所有语句全都缩进
  如果try中的有错误，则直接转到except中的语句
  '''
  try:
      fahr = float(inp)
      cel = (fahr - 32.0) * 5.0 / 9.0
      print(cel)
  
  '''
  如果try中有错误，则执行except
  如果try没错，则跳过except
  '''
  except:
      print('Please enter a number')
  ```

- try中要尽量少放代码（只放可能有问题的代码）

  ```python
  # 练习题要求 ex_3.2 https://www.py4e.com/lessons/logic
  
  hrs = input("Enter Hours: ")
  try:
      h = float(hrs)		# try之中只放少量代码
  except:
      print ('Error, please enter numeric input')
      quit()      		# 如果执行完except发现错误，则直接终止程序，后面的流程不再走
  
  rate = input ('Enter Rate: ')
  try:
      r = float (rate)	# try之中只放少量代码
  except:
      print ('Error, please enter numeric input')
      quit()      		# 如果执行完except发现错误，则直接终止程序，后面的流程不再走
  
  if h <=40:
      salary = r * h
  else:
      salary = (r * 40) + (1.5 * r * (h - 40))
  print (salary)
  ```

## 测试题

- [py4e测试题(同coursera)](https://www.py4e.com/lessons/logic)

# Week 6 - Function

## 参考书

- [英文版](https://books.trinket.io/pfe/04-functions.html)

## 笔记

### 调用函数

- function的本质是将一组操作固定成一个模块，之后再用这组操作的时候直接调用模块即可（不用每次都重新写各种操作）

  - function属于store and reuse

- function实质性computation的named sequence of statement

- 函数中的表达式是函数的argument

- 函数会接收一个argument，并返回一个result（返回值）

  ```python
  >>> type(32)	# 32是函数中的argument
  <class 'int'>
  ```

### Built-in Function（BIF）

- max() 和 min()

  ```python
  >>> max('Hello world')	# 取内容的最大值
  'w'
  >>> min('Hello world')	# 取内容的最小值
  ' '
  ```

- len(): 返回参数中有多少个字符

  ```python
  >>> len('Hello world')
  11
  ```

### 转换数值类型的函数

- int(): 转化为整数

  ```python
  >>> int(3.99999)	# int()转化浮点数时，直接去小数点后的部分，只保留整数位
  3
  >>> int(-2.3)		# int()转化浮点数时，直接去小数点后的部分，只保留整数位
  -2
  ```

- float()

  ```python
  >>> float(32)
  32.0
  >>> float('3.14159')
  3.14159
  ```

- str()

  ```python
  >>> str(32)
  '32'
  >>> str(3.14159)
  '3.14159'
  ```
  
- 错误转换或未转换时，可能会发生错误

  ```python
  # 字符串和数字之间不能运算
  >>> sval = '123'
  >>> type(sval)
  <class 'str'>	# 说明sval变量的数值类型为str
  >>> print (sval +1)	# 此处属于str加int，所以下面会报错
  Traceback (most recent call last):
    File "<pyshell#24>", line 1, in <module>
      print (sval +1)
  TypeError: can only concatenate str (not "int") to str
  ```

  

### 随机数 (random number)

- 可使用算法生成伪随机数（pseudorandom number）
  
  - Pseudorandom number不是真正的随机数，而是由确定的计算产生的（但是看起来像是随机数）
  
- random module中有函数可以生成伪随机数

- 先要导入random module，之后再使用其中的函数

  ```python
  # 导入random模块
  import random
  ```

  

#### random.random()

- random.random()是生成[0,1)之间的随机数

  ```python
  # 此步骤导入random module
  >>> import random
  
  # 使用random模块中的random()函数生成随机数并打印
  # 使用模块中的函数的语法为模块名.函数名()，如random.random()
  >>> print (random.random())	# random.random()是生成[0,1)之间的随机数
  0.99010304321227
  >>> print (random.random())
  0.1879765138773849
  >>> print (random.random())
  0.4001109938840649
  ```


#### random.randint()

- random.randint()是生成制定区域（含）之间的整数

  ```python
  >>> random.randint(5, 10)
  5
  >>> random.randint(5, 10)
  9
  ```

#### random.choice()

-  random.choice()是从给定的序列中随机选择一个元素

  ```python
  # 先给出序列（用以从中随机挑选一个值）
  # 序列用[]括起来
  t = [1,2,3,5,6,7,8,23,3254,1234,2354,1234]
  
  # 使用random.choice(),从已定义的序列中随机取出一个值
  >>> random.choice (t)
  5
  ```

#### random module中的其它功能

- random module还包括其它函数，如为各种分布产生random value

### 数学相关的函数

- 要使用模块中的函数，必须在代码中写上module.function()

  ```python
  # 导入math模块
  import math
  
  ratio = signal_power / noise_power
  decibels = 10 * math.log10(ratio)	# 此处使用module中的函数，格式为module.function()
  radians = 0.7
  height = math.sin(radians)
  ```

- $\pi$的表达式： 可从math module中，获得$\pi$的值(近似到15位)

  ```python
  >>> import math
  >>> math.pi
  3.141592653589793
  ```

### 自定义新函数

- 除去python自带函数外，还可以自行添加新函数

- 定义新函数时，需确定新函数的name和sequence of statement

  ![](https://s3.ax1x.com/2020/12/03/Do2LFA.jpg)

  ```python
  # 定义新函数
  >>> def thing():	# 新函数的header。定义了一个新函数，新函数名字是thing
      
      # 新函数的body(需要缩进), body中只有两行代码
  	print ('hello')
  	print ('fun')
      
  # 测试新定义的函数
  >>> thing()	# 遇到新定义的函数时，找到已定义好的函数，执行，并输出结果
  hello
  fun
  ```

- 自定义新函数

  - 语法为def function_name(参数):
    - def是说明要定义一个新函数
    - 函数命名规则和variable一样，不能使用reserved word
    - 括号中是参数（也可以没有参数）
  - 函数的第一行为header，其他行为body（必须缩进）
  - 结束定义函数时，需要输入一个空行
  - 可以只定义新函数，但不执行新函数（此时只是将函数储存起来）。只有调用函数时，新定义的函数才会执行

- 定义函数后，python会创建和函数名一样的变量

- 可以在新函数中，使用已经定义的函数（既可以嵌套定义函数）

- 自定义新函数案例

  ```python
  # 自定义一个新函数
  # 语法为def function_name(参数):
  
  def print_lyrics():	# def是说明要定义一个新函数。函数命名规则和variable一样。括号中是参数（也可以没有参数）。
      print("I'm a lumberjack, and I'm okay.")	# 函数的body必须缩进
      print('I sleep all night and I work all day.')
      	# 结束定义函数时，必须输入一个空行
  ```

  ```python
  # 测试新定义的函数（新函数的使用方法和变量一样）
  >>> print_lyrics()	# 此处要加括号，以显示函数内容
  I'm a lumberjack, and I'm okay.
  I sleep all night and I work all day.
  ```

  ```python
  # 查看新函数的位置
  >>> print(print_lyrics)
  <function print_lyrics at 0xb7e99e9c>
  
  
  # 定义好新函数后，python会创建一个同名的变量
  >>> type (print_lyrics)
  <class 'function'>
  ```

  ```python
  # 函数的嵌套定义
  >>> def repeat_lyrics():	# 定义函数时，必须有()和:
  		print_lyrics()		# 新函数的body使用之前已定义的函数
  		print_lyrics()
  		print_lyrics()
          
  # 测试新定义好的嵌套函数
  >>> repeat_lyrics()			# 此处必须写完全的函数名，即function_name()
  I'm a lumberjack, and I'm okay.
  I sleep all night and I work all day.
  I'm a lumberjack, and I'm okay.
  I sleep all night and I work all day.
  I'm a lumberjack, and I'm okay.
  I sleep all night and I work all day.
  ```

### 定义和用途

- 使用自定义函数前，必须先定义函数

### 执行流程

- 函数不会改变程序的执行流程（程序一直都是从上向下依次执行）
- 碰到函数时，程序会暂停，之后跳到函数定义的地方执行函数，得到函数的结果后，把结果带回到刚才暂停的地方，之后继续执行程序
  - 所以相应的，看程序的时候也要来回跳着看（跟随执行流程看）

### 参数

- 自定义的函数中，可以加入参数

  ![](https://s3.ax1x.com/2020/12/03/Do2zy8.jpg)

  - parameter是被赋值的argument
  - ‘hello world’ 是argument
  - 先用max (‘hello world’)计算出结果‘w’（‘w’是max()的返回值）
  - 之后将‘w'赋值给变量big，此时big的值就是‘w’

- 函数中的参数

  ```python
  # 在自定义的函数中加入参数
  def print_twice(bruce):	# 函数将argument赋给parameter，此处为bruce
      print(bruce)
      print(bruce)
      
  # 测试新定义的函数
  # 不管被赋予什么样的值，都会执行print语句2次
  >>> print_twice('Spam')	
  Spam
  Spam
  >>> print_twice(17)
  17
  17
  
  # 只要()中有值（不管是什么类型），都会执行print_twice()
  >>> import math
  >>> print_twice(math.pi)
  3.141592653589793
  3.141592653589793
  
  >>> print_twice('Spam '*4)	# ()里是表达式也可以。此时程序先计算'Spam' * 4, 得到值，之后将这个值再放到print_twice()函数中，之后再执行函数
  Spam Spam Spam Spam
  Spam Spam Spam Spam
  
  >>> print_twice(math.cos(math.pi))	# 先计算math.cos(math.pi)的值，获得结果后，将结果放到print_twice()函数中，再执行函数
  -1.0
  -1.0
  ```

  ![](https://s3.ax1x.com/2020/12/03/Do4g8s.jpg)

### fruitful function和void function

- fruitful function是可以产生result（即内部有计算公式，或return statement会返回function result）的函数（如math function）

  ```python
  # 交互环境下调用fruitful function时，会直接显示结果
  >>> math.sqrt(5)
  2.23606797749979
  
  # print fruitful function时，返回值为计算好的值（和直接用函数效果一样）
  >>> print (math.sqrt(5))
  2.23606797749979
  ```

  

- void function是只执行操作，不会返回值的函数（如只执行print操作的函数）

  ```python
  # void function中，没有计算公式，也没有返回值
  >>> result = print_twice('Bing')
  Bing
  Bing
  
  # print void function时，返回值为None
  >>> print(result)
  None	# None属于一种特殊的值，不是字符串（不是'None'）
  
  # 值 None 与字符串“ None”不同，其有自己的类型
  >>> print(type(None))
  <class 'NoneType'>
  ```

- 可使用return语句返回结果

  ```python
  # 定义新函数，使用return返回结果
  >>> def addtwo (a, b):
  	add = a + b			# 函数的主体
  	return add			# 使用return返回结果
  
  >>> x = addtwo (13, 5)	# 使用新定义好的函数，13和5为参数
  >>> print (x)	# 
  18
  ```
  
  ```python
  # 使用return返回结果
  >>> def great ():			# 定义一个新函数
  	return 'hello'			# 让函数返回一个值，为'hello'
  
  >>> print (great(), 'Glen')	# 碰到函数时，程序会先执行函数（这步中是得到一个值'hello'），之后执行print ('hello', 'Glen')
  
  hello Glen
  ```
  
  

### function的优点

- 可以命名一组代码（让程序变的更小）
- 可以复用
- 将程序分解为多个函数，可使用函数组装程序

### debug

- 要注意tab和4个空格的问题

## 测试题

- [测试题](https://www.py4e.com/lessons/functions)

# Week 7 - Loops and Iteration

## 参考书

- [英文版](https://books.trinket.io/pfe/05-iterations.html)

## 笔记

### 更新变量

- 可对变量进行更新，即使用新值替代变量中的旧值

  ```python
  # 更新变量的值
  x = x + 1	# 先获取当前的x值，在此基础上 +1，之后将新值再赋给x
  
  # 更新变量前，必须先定义变量，否则报错
  >>> x = x + 1
  NameError: name 'x' is not defined
  ```

- +1 是递增（increment）
- -1 是递减（decrement）

### while

- while属于无限循环（indefinite loop）

- while案例

  ```python
  # 倒数，满足特定条件后，打印特定词语
  # 当 n 大于0时，显示 n 的值，然后将 n 的值减少1。当数到0时，退出 while 循环，显示单词 Blastoff!
  
  n = 5			# 先赋值
  while n > 0:	# 确定while语句的判断条件。如果条件为真，则继续执行代码块中的内容。如果条件为假，则跳过代码块（功能类似if语句，如果真，则执行代码块，如果假，则跳过代码块）
      print (n)	# 代码块中写要执行的内容。此处注意缩进
      n = n - 1	# while代码块中，必须有一段要改变变量的值，以防其无限循环。此处n属于iteration variable（每循环一次，就改变一次值）。执行完成后，继续回到while条件判断处（此处和if语句不一样，if不会跳回，而是继续向下执行代码）
  print ('Blastoff!')
  ```

  - 执行步骤

    ![](https://s3.ax1x.com/2020/12/03/DHC4cn.jpg)

- while的执行流程
  - 评估条件的真假，产生True/ False
  - 如果条件为True，则继续执行while代码块中（缩进部分）的内容。执行完代码块中的内容后，回到while的第一行，重新判断
    - 每执行完一次（称为迭代），程序都会回到while语句
    - 每执行一次，都属于一次迭代
    - while评估条件中，必须和变量值相关
    - 代码块中必须有一段要改变变量的值，以防其无限循环
      - 如果while中的条件判断结果一直是True，则其会一直循环下去（所以while属于无限循环）
      - 需要设定一个iteration variable，用以控制循环
  - 如果条件为False，则跳过代码块（缩进部分），继续执行

### 无限循环和break

- 无限循环的while语句

  ```python
  # 无限循环的while语句
  n = 10
  while True:		# while后的条件一直是True，程序会在while的代码块中无限循环。while的判断条件中，必须和变量的值相关
      print(n, end=' ')
      n = n - 1	# 即使有改变变量的语句，但是对判断本身无用（因为一直都是True）
  print('Done!')
  ```

  ![](https://s3.ax1x.com/2020/12/03/DHiDdf.jpg)

- 有的循环是无限的，因为没有要迭代的变量（iteration variable）

- 可使用break跳出无限循环

  ```python
  # 使用break跳出无限循环
  # 可使用http://pythontutor.com/演示流程
  
  while True:				# 确定while的判断条件，此处条件一直是True，即代码块中的代码会一直执行
      line = input('> ')	# 让客户输入值
      if line == 'done':	# 如果客户输入的值是'done'，则执行if代码块中的语句，如果不是，则执行else语句
          break			# 停止执行while代码块，直接跳过while代码块中的所有内容，执行下一步程序
      else:
          print (line)	# 如果客户输入的值不是'done'，则执行此语句
  print ('Done!')
  
  # 执行后的情况
  > hello there
  hello there
  > finished
  finished
  > done
  Done!
  ```

- 有的循环属于0循环，即不会执行代码块中的内容（因为未满足while的条件）

  ![](https://s3.ax1x.com/2020/12/03/DHi4e0.jpg)

  

### continue

- continue是停止当前的迭代，直接跳到下一个迭代（循环），但不跳出循环

  ```python
  # continue会停止当前的迭代，直接进入下一个迭代
  # 可使用http://pythontutor.com/演示流程
  
  while True:
      line = input ('> ')
      if line [0] == '#':	# 如果输入的值的第一个字符为#，则进入if为true的代码块
          continue		# continue说明结束当前的迭代，不再向下执行语句，回到while判断
      if line == 'done':	# 如果输入值为done，则进入以下if代码块
          break			# break说明终结现在所有的while代码块，跳过剩余的所有 代码块（跳出while循环），直接进入到print ('Done!')
      print (line)
  print ('Done!')
  ```
  
  ![](https://s3.ax1x.com/2020/12/03/DHF7HP.jpg)
  
- continue和break的区别

  - continue只是跳出此次循环，转到下一次循环
  - break是直接结束所有循环，开始执行循环之后的语句

### for

- for可用于遍历一组事件，不管逻辑判断，所以其for的迭代次数（运行次数）和集合中的元素数一样多

  - for属于definite loop

- for和while区别在于

  - while是只有条件判断为真时，才执行while代码块
  - for是不管条件判断，把事物中的所有元素都过一遍

- for的语法

  - 先定义好一个集合
- for 变量 in 集合:
    - for ‘variable’ in ‘list’: 执行下列代码
  - 确定要执行的代码（for循环的body）

- for循环中也可使用break和continue

- for案例

  ```python
  # for是把集合中的所有元素都过一遍，不管逻辑判断（此处和while有区别）
  friends = ['Joseph', 'Glenn', 'Sally']		# 变量friends中，有3个字符串组成的list
  for friend in friends:						# 此处定义了变量friend（属于iteration variable），说明变量friend是变量friends的一个子集。可解释为对于每一个在friends中的friend，都执行代码块中的语句。for和in都是reserved word
      print('Happy New Year:', friend)		# 对每个元素，都执行一遍代码块中的所有语句
  print('Done!')								# 只有遍历完所有变量中的元素后，才推出for循环，进入到下一个语句
  ```

  ```python
  # 和while中的案例效果一样，但简化了很多
  for i in [5,4,3,2,1]:
      print (i)
  print ('blastoff')
  ```
  
  ![](https://s3.ax1x.com/2020/12/03/DHAkZt.jpg)

### loop pattern

- 循环通常由以下元素构成
  - 循环开始前有1个已定义的变量（用于计数）
  - 每执行一次循环，就改变一次变量的值（控制循环的次数）
    - 每一次循环完成，都让结果能更接近答案（但不会直接得到答案）
  - 循环完成时，得到结果

#### count loop

- 用于计数的循环

  ```python
  # 计算列表中有多少个数
  
  count = 0								# 循环开始前，定义好一个变量（初始值）。此处用于计数，所以初始值为0
  for itervar in [3, 41, 12, 9, 74, 15]:	# 因为要计算列表中有多少个数，所以要使用for语句。此句中，定义了变量itervar（属于iteration variable，只用一次的临时变量，后面不再用，只是为了满足for中循环的要求），确定了集合[3, 41, 12, 9, 74, 15]
      count = count + 1					# 对集合中，每个元素要执行的代码。count初始值为0，每进行一次循环，则count的值增加1（即计数的流程就是看有多少次循环）
  print('Count = ', count)
  ```

#### sum loop

- 用于求和的循环

  ```python
  # 计算集合中的值，总和是多少
  # 和计数的for循环类似，知识改变了body中的公式
  
  total = 0							# 循环开始前，定义好一个变量（初始值）。此变量用于求和，所以初始值为0
  for t in [3, 41, 12, 9, 74, 15]:	# t是临时变量，是为了满足for语句的格式，也用于从集合中取数
      total = total + t				# 每执行一次循环，则执行一次相加操作。没执行一次循环，total的值会变化（在前一次total值的基础上增加t），即total是一个累加器。此处和计数的for循环有区别（但只有此处的区别）
  print ('sum =', total)				# 遍历完集合中的所有值后，输出total的值
  ```
#### average loop

- 用于计算均值的loop

  ```python
  # 用于计算集合的均值（到目前为止的均值）
  # 综合了上述的sum loop和count loop，需要一个总和值，一个计数值
  total = 0								# 求和值的起始值设定为0		
  count = 0								# 计数值的起始值设定为0
  for t in [3, 41, 12, 9, 74, 15]:		# iteration varriable用于控制循环和取数
      count = count + 1					# 每循环一次，计数值+1
      total = total + t					# 每循环一次，求和值在初始值的基础上 + t取到的值
      avg = total / count					# 计算当前迭代完成后的平均值
  print ('average =', avg)				# 输出结果
  ```

#### maximum loop

- 找集合中的最大值

  ```python
  # 找集合中的最大值
  
  largest = None				# 初始量设定为None（特殊的常量，类似于空置）
  for t in [3, 41, 12, 9, 74, 15]:
  
  '''
  以下步骤也可简化
  '''
  
      if largest is None:		# None值无法比大小，此时是直接给largest赋值为第一个t
          largest = t			# 直接将现有的t值赋给变量largest
      elif t > largest:		# 如果t值大于largest，则用现在的t值更新largest的值
          largest = t			# 用t值更新largest值
  print('Largest:', largest)	# 输出结果
  ```

  - 简化的步骤

    ```python
    # 找集合中的最大值（简化）
    
    largest = None
    for t in [3, 41, 12, 9, 74, 15]:
        if largest is None or t > largest:	# 此处进行了简化
            largest = t
    print('Largest:', largest)
    ```

  ```python
  # 简化理解的版本
  
  largest = -10000000						# 随意设定一个特别小的值，作为初始值
  for number in [3, 41, 12, 9, 74, 15]:	# 让number遍历列表中的所有项
      if number > largest:				# 判定条件
          largest = number				# 如果满足判定条件，则更新初始值
  print ('largest number is', largest)
  ```

#### minimum loop

- 找集合中的最小值

  ```python
  smallest = 999999999		# 随便赋一个巨大的值(此处只是为了简化问题，不是正确的写法)
  for t in [3, 41, 12, 9, 74, 15]:
      if t < smallest:
          smallest = t
  print ('smallest:', smallest)
  ```

- 常规写法（使用None）

  ```python
  smallest = None					# None是循环中的初始值，只用在第一次循环中
  for t in [3, 41, 12, 9, 74, 15]:
      if smallest is None:		# 此处说明之第一次循环（将变量和None作比较）。可使用is，也可使用==
          smallest = t
  	elif t < smallest:			# 第二次和以后的循环时，不在对比None
          smallest = t
  print ('smallest is :', smallest)
  ```

- python中min()的写法

  ```python
  def min(values):
      smallest = None
      for value in values:
          if smallest is None or value < smallest:
              smallest = value
      return smallest
  ```

- is和is not

  - is是比较两个值是否完全相同（即is the same as）。is比==更强
  - 一般只有判断True/ False时，才使用is或is not

#### 对loop中的值进行筛选

- 使用if语句，对集合中的元素进行筛选

  ```python
  # 选出集合中所有大于20的值
  
  for v in [3, 41, 12, 9, 74, 15]:		# 用iteration variable控制循环，并取数
      if v > 20:							# 判断条件
          print ('large number:', v)		# 对每次循环执行该语句
  ```

- 使用布尔值，判断集合中每个值的情况

  ```python
  # 使用布尔值，判断集合中有没有15，并计数
  
  count = 0						# 计数的初始值为0
  for v in [3, 41, 12, 9, 74, 15]:
      if v == 15:					# 此处要用==，而非=，小心
          print ('15 found')		# 如果有15，则打印
          count = count + 1
  if count == 0:					# 一定注意，判断是不是等于时，要使用==，而非=
      print ('there are no 15 found')
  else:
      print ('there are', count, '15 in the dataset')
  ```

### debug

- 如果运行程序时报错，则可使用二分法找错误所在
- print() 二分法
  - 在可能出错的地方或附近，找个地方加入print()语句（输出一下当前各变量的值）
    - 如果print()的结果不对，则问题在print()之前的部分
    - 如果print()的结果正确，则问题在print()之后的部分
  - 持续使用二分法6-7次后，可基本确定错误的位置
- 二分法不一定必须用在最中间的地方，任何可发生错误的地方都可使用二分法

## 测试题

### ex_5.1

#### 要求

Exercise 1: Write a program which repeatedly reads numbers until the user enters “done”. Once “done” is entered, print out the total, count, and average of the numbers. If the user enters anything other than a number, detect their mistake using try and except and print an error message and skip to the next number.

```python
Enter a number: 4
Enter a number: 5
Enter a number: bad data
Invalid input
Enter a number: 7
Enter a number: done
16 3 5.333333333333333
```

#### 解答

```python
# 根据输入的值，计算sum, count和average
total = 0								# 作为累加器，total的初始值为0
count = 0								# 作为累加器，count的初始值为0
while True:								# 此处引入循环（因为循环没有判定条件，所以使用单一值，让循环一直持续下去）
    number = input ('Enter a number: ')	# 让用户输入值
    if number == 'done':				
        break							# 如果用户输入值为done，则结束整个while循环
    try:								# 增加可能的报错判断
        fn = float (number)				# 如果输入值没问题，则将其转化为小数
    except:
        print ('Invalid input')			# 如果有错时，要执行的语句（提示用户输入有错）
        continue						# 停止当前循环，返回到while判断，重新开始循环
    total = total + fn					# 累加器
    count = count + 1					# 累加器
    avg = total / count					# 计算均值
try:
    print ('total =', total, 'count =', count, 'average =', avg)		# 如果都没问题，则输出结果
    print ('all done')
except:																	
    print ('nothing input')												# 如果输入有问题，则输出另一个结果
```

### ex_5.2

#### 要求

Exercise 2: Write another program that prompts for a list of numbers as above and at the end prints out both the maximum and minimum of the numbers instead of the average.

#### 解答

```python
# 根据输入的值，计算sum, count和average

# 设定初始值
total = 0								# 作为累加器，total的初始值为0
count = 0								# 作为累加器，count的初始值为0
maximum = None
minimum = None

# 引入循环
while True:								# 此处引入循环（因为循环没有判定条件，所以使用单一值，让循环一直持续下去）
    number = input ('Enter a number: ')	# 让用户输入值
    
    # 判断输入的值是否符合要求
    if number == 'done':				
        break							# 如果用户输入值为done，则结束整个while循环
    try:								# 增加可能的报错判断
        fn = float (number)				# 如果输入值没问题，则将其转化为小数
    except:
        print ('Invalid input')			# 如果有错时，要执行的语句（提示用户输入有错）
        continue						# 停止当前循环，返回到while判断，重新开始循环
	
    # 计算sum, count和average
    total = total + fn					# 累加器
    count = count + 1					# 累加器
    avg = total / count					# 计算均值
	
    # 判断最大值
    if maximum is None:					# 第一次判断
        maximum = fn
    elif fn > maximum:					# 比较当前值和maximum
        maximum = fn					# 给maximum赋值

    # 判断最小值
    if minimum is None:
        minimum = fn
	elif fn < minimum:					# 比较当前值和minimum
        minimum = fn					# 给minimum赋值

# 输出结果
try:
    print ('total =', total, 'count =', count, 'average =', avg, 'minimum =', minimum, 'maxixmum =', maximum)	# 如果都没问题，则输出结果
    print ('all done')
except:																	
    print ('nothing input')																						# 如果输入有问题，则输出另一个结果
```

