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

### 1. 数据类型和变量

**整数**：也就是数学上的整数，1,100,23

**浮点数**：有小数点的数，2.3333

**字符串**：是以单引号`'`或双引号`"`括起来的任意文本，但如果输出包含了单引号`'`，就需要用转义字符`\`来标识。就需要插在需要显示的引号前面

	>>>print('I \'m \"OK\"!')
	I 'm "OK"!

转义字符也有其他用法，`\n`用来换行，`\t`表示制表符，不过还没用过这个，由于`\`本身也需要转义，所以用`\\`来表示`\`。还有用`'''`来输出多行。

廖雪峰教程里还说了**布尔值**，就是`True`和`Flase`，和高中学命题的差不多，`and`是真真才真，`or`是一真则真，`not`就是非。

还有**空值**，是`none`，不过说得不多，空值没意义。

**变量**就是用`=`去赋予值，可以用大小写字母、`_`、数字等，如`a = 100`，`C_187 = 23333`，但不能用数字开头。

**常量**就是不能变的量，这个没太懂。不过还说了两种除法，一是用`/`，结果是浮点数；而是用`//`，称为地板除，只取整数。要算的精确用`/`，要整数用`//`。

	>>>10 / 5
	2.0
	>>>10 / 3
	3.3333333333333335
	>>>25 // 5
	5
	>>>50 // 6
	8

最后留了一个题，还挺简单的，要求打印下面变量的值：

	n = 123
	f = 456.789
	s1 = 'Hello, world'
	s2 = 'Hello, \'Adam\''
	s3 = r'Hello, "Bart"'
	s4 = r'''Hello,
	Lisa!'''

做了一下，对啦，主要是多用用`\`就好了。

	print('''n = 123
	f = 456.789
	s1 = \'Hello, world\'
	s2 = \'Hello, \\'Adam\\'\'
	s3 = r\'Hello, \"Bart\"\'
	s4 = r\'\'\'Hello, 
	Lisa!\'\'\'''')
上面是2018/7/24 21:11的笔记。
