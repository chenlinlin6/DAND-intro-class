1.关于python的赋值，左边可以不加下划线写成animal lion='lion' 这样的形式吗？

> 不可以。变量名只能以字母，数字，下划线构成，中间不能出现空格。

2.pandas的dataframe某一列名为'City'，我想抽取该列，写成df['city']，返回key error:city的报错，请说下你理解的为什么会报这个key error这个错误？

> city和City的大小写不一样，所以会报错

3.什么是箱线图？你认为上面的几个重要指标分别是什么？

> 箱线图（Boxplot）也称箱须图（Box-whisker Plot），是利用数据中的五个统计量：最小值、第一四分位数、中位数、第三四分位数与最大值来描述数据的一种方法，它也可以粗略地看出数据是否具有有对称性，分布的分散程度等信息，特别可以用于对几个样本的比较。

4.python当中的try和except语句是什么用途？

> try/except语句用来检测try语句块中的错误，从而让except语句捕获异常信息并处理。

5.常用的逻辑判断符号有哪些？比如"=="检验两个变量是否相等，">"表示大于

> ==	等于 - 比较对象是否相等
>
> !=	不等于 - 比较两个对象是否不相等
>
> <>	不等于 - 比较两个对象是否不相等
>
> \> 大于 - 返回x是否大于y
>
> <	小于 - 返回x是否小于y。所有比较运算符返回1表示真，返回0表示假。这分别与特殊的变量True和False等价。
>
> =	大于等于	- 返回x是否大于等于y。
>
> <=	小于等于 -	返回x是否小于等于y。

6.现在有一个文本字符串是s='string'，请问s.split('i')返回的结果是什么？s.split('i')[0]呢？

> 6_1  s.split('i')返回的结果是['str', 'ng'];6_2  s.split('i')[0]返回的结果是str ;  6_3语法：str.split(str="",num=string.count(str))[n]
> 参数说明：str表示为分隔符，默认为空格，但是不能为空('')。若字符串中没有分隔符，则把整个字符串作为列表的一个元素;num表示分割次数。如果存在参数num，则仅分隔成 num+1 个子字符串，并且每一个子字符串可以赋给新的变量;[n]表示选取第n个分片

7.print 'hello\n'，这个语句显示的结果中\n有没有显示出来？\n是普通的文本吗？

> \n没有显示，它表示换行 不是普通文本 ，\是转义

8.集合里面的元素是唯一的吗？

> 集合里面的元素是唯一的

9.假如你不知道pandas如何去除一列里面的重复值，你会如何在谷歌搜索这个方法？(用英文)

> python pandas remove duplicate value in column

10.dewp=20   print 'The missing number of DEWP is %d'%20。显示的结果是什么？如何用format和{}实现相同的显示结果？

> 显示的结果为 The missing number of DEWP is 20;等价写法: print("The missing number od DEWP is {}".format(20))

11.pandas删除缺失值用什么方法？是在原本的dataframe上面修改的吗？

> ```python
> import pandas as pd
> 
> import numpy as np
> 
> df = pd.DataFrame(np.random.randn(5, 3), index = list('abcde'), columns = ['one', 'two', 'three'])        # 随机产生5行3列的数据    
> 
> df.ix[1, :-1] = np.nan        # 将指定数据定义为缺失
> 
> df.ix[1:-1, 2] = np.nan print('\ndrop row')
> 
> print(df.dropna(axis = 0))
> 
> ```

12.如何查看一个dataframe里面有多少条数据？

> 使用len（）函数或者describe（）函数

13.python的模块是什么后缀名的文件？我们是否也可以自己写一个模块并导入？

> .py模块可以自己编写并导入。

14.现在有个字典phonebook   = {"John" : 938477566,"Jack" : 938377264,"Jill"   : 947662781}，我想依次打印出每个键和对应的值，怎么写？（提示：iteritems()）

> for key in  phonebook:
>            print(key, phonebook[key])

15.如何用lambda写一个将输入值x转化成x的平方的函数（了解lambda定义函数的基本语句）

> ```python
> square=lambda x:x**2
> ```

