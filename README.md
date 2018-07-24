# python 笔记
学python时候，记一些笔记，顺带写写自己的思考。
## 第一个python程序
    >>>print('hello, world')
    hello, world
第一个程序，还是很简单的。

	cd C:\Users\name\Downloads
cd是用来切换当前命令行的盘符，看廖雪峰的教程时，折腾半天，才知道怎么去打开learning.py

	C:\Users\name\Doenloads>python learning.py
然后就可以在命令行模式下，输入 python打开learning.py这个文件辣

	>>>print('100 + 200 =', 100 + 200)
	100 + 200 = 300
这里面的`'100 + 200 ='`是字串符不是公式，和前面`'hello, world'`同理，用来显示输出

	
	name = input()
	Michael
这里面name是个变量，就把`Michael`存在name里面，所以可以这样

	>>>print('hello,', name)
	hello, Michael
就可以玩一个高级的，用Notpad++输入代码，另存为hello.py

	name = input('please enter your name: ')
	print('hello,', name)
运行之后，会先打印出`please enter your name:`，键入名字，就得到`hello, xxx`

	C:\work>python hello.py
	please enter your name: Michael
	hello, Michael
有输入才有输出，`input()`是输入，`print()`是输出

## Python基础
**整数**：也就是数学上的整数，1,100,23

**浮点数**：有小数点的数，2.3333

**字符串**：是以单引号`'`或双引号`"`括起来的任意文本，但如果输出包含了单引号`'`，就需要用转义字符`\`来标识。就需要插在需要显示的引号前面

	print('I \'m \"OK\"!')
	I 'm "OK"!
