# python
跟着Micheal Liao的教程学python

###在线输入Python代码
cd C:\Users\hust\Downloads
python learning.py



###输入输出

name = input('please enter your name: ')			
print('hello,', name)

我们把输入输出统称为Input/Output，或者简写为IO

当语句以冒号:结尾时，缩进的语句视为代码块。

应该始终坚持使用4个空格的缩进。

Python程序是大小写敏感的，如果写错了大小写，程序会报错。 

在文本编辑器中，需要设置把Tab自动转换为4个空格，确保不混用Tab和空格。



###数据类型和变量

浮点数也就是小数 把10用e替代，1.23x109就是1.23e9，或者12.3e8，0.000012可以写成1.2e-5

n = 123
f = 456.789
s1 = 'Hello, world'
s2 = 'Hello, \'Adam\''
s3 = r'Hello, "Bart"'
s4 = r'''Hello,
Lisa!'''
print(n,f,s1,s2,s3,s4,sep='\n')

print(r'''I'm telling you that "Python is Great"''')

在计算机内部，可以把任何数据都看成一个“对象”，而变量就是在程序中用来指向这些数据对象的，对变量赋值就是把数据和变量给关联起来。



###字符串和编码

8个比特（bit）作为一个字节（byte）

>>> '中文'.encode('utf-8')
b'\xe4\xb8\xad\xe6\x96\x87'

格式化：
>>> 'Hi, %s, you have $%d.' % ('Michael', 1000000)
'Hi, Michael, you have $1000000.'



###使用list和tuple

list是python的一种数据类型，是一种有序的集合

tuple和list非常类似，但是tuple一旦初始化就不能修改

要定义一个只有1个元素的tuple必须加一个逗号,，来消除歧义：

>>> t = (1,)
>>> t
(1,)
Python在显示只有1个元素的tuple时，也会加一个逗号,，以免你误解成数学计算意义上的括号。



###条件语句

elif是else if的缩写

这是因为input()返回的数据类型是str，str不能直接和整数比较，必须先把str转换成整数。Python提供了int()函数来完成这件事情



###循环

字符串之间用+号连接可以避免产生空格



###使用dict和set

dict全称dictionary，在其他语言中也称为map，使用键-值（key-value）存储，具有极快的查找速度。

需要牢记的第一条就是dict的key必须是不可变对象

一是通过in判断key是否存在：

>>> 'Thomas' in d
False
二是通过dict提供的get方法，如果key不存在，可以返回None，或者自己指定的value：

>>> d.get('Thomas')
>>> d.get('Thomas', -1)
-1
注意：返回None的时候Python的交互式命令行不显示结果。


在Python中，字符串、整数等都是不可变的，因此，可以放心地作为key。而list是可变的，就不能作为key

猜想：set是把list变为集合的工具

dict是函数，上例的d是一个dict的名字



###函数

pass表示什么也不做

positional argument的意思是位置参数

如果你已经把my_abs()的函数定义保存为abstest.py文件了，那么，可以在该文件的当前目录下启动Python解释器，用from abstest import my_abs来导入my_abs()函数，注意abstest是文件名（不含.py扩展名）：

函数体内部可以用return随时返回函数结果；

函数执行完毕也没有return语句时，自动return None。

函数可以同时返回多个值，但其实就是一个tuple。



###函数的参数

可变参数允许你传入0个或任意个参数，这些可变参数在函数调用时自动组装为一个tuple。而关键字参数允许你传入0个或任意个含参数名的参数，这些关键字参数在函数内部自动组装为一个dict。

定义位置参数def calc(numbers):
传列表nums用calc(nums)
定义可变参数def cal(*numbers):
传列表nums用calc（×nums）
可变参数的函数传列表list可以直接用calc(1,2,3,4)

命名关键字参数必须传入参数名，这和位置参数不同。如果没有传入参数名，调用将报错
但是输出的是赋值给参数名的内容
而关键字参数输出的是 参数名-赋值给参数名内容 的dict
这里的参数名好像只能用str



