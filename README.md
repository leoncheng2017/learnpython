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




