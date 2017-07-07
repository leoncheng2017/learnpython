# python
跟着Micheal Liao的教程学python

name = input('please enter your name: ')			
print('hello,', name)

我们把输入输出统称为Input/Output，或者简写为IO

当语句以冒号:结尾时，缩进的语句视为代码块。

应该始终坚持使用4个空格的缩进。

Python程序是大小写敏感的，如果写错了大小写，程序会报错。 

在文本编辑器中，需要设置把Tab自动转换为4个空格，确保不混用Tab和空格。




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
