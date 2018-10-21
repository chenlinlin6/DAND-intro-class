1.python的import语句是实现什么功能？  
> 用于动态加载类和函数

2.pandas是一个什么工具包？  
> pandas是python的第三方库，可以快速处理数据集，建立DataFrame  
> · 基于Numpy建立的开源库  
> · 快速进行数据分析，数据清理等一系列数据准备工作  
> · 有自带的数据可视化特征  

3.%matplotlib inline这个语句实现什么功能？
> 可以使得matplotlib绘制的图形在jupyter notebook直接显示

4.pandas怎么样取出名为表格第二行数值？怎么样取出字段名为‘city’的这一列？
> df[1]; df['city']

5.数据异常值通常是指哪几种情况？
> 数据异常(outliers), 是分析数值类型数据的四大方面之一, center, spread, shape, outliers. 有时候数据集中会包含一个或多个数值异常大或异常小的值，这样的极端值称为异常值（outlier）。
因此主要有两种情况, 异常大, 和异常小

6.csv文件是以什么分隔的文件？
> csv文件是以逗号或制表符分隔的文件。csv是comma-separated values 的简称。csv文件以纯文本形式存储表格数据。

7.我们一般会查看数值数据（也就是字段都是数字）的哪些统计学变量？比如平均值
> 平均值 中位数 众数 方差 标准差

8.python当中的out_columns = ['No', 'year', 'month', 'day']，请问我打印out_columns，接下来会显示什么内容？
> 显示 ['No', 'year', 'month', 'day']

9.数据当中的NaN是什么意思？
>NaN，是number类型，是Not a number的缩写，代表非数字值的特殊值。数据处理时，在实际工程中数据的缺失或者不完整，此时我们可以将那些缺失设置为nan。

10.pandas的read_csv模块作用是什么？  
city_data = pd.read_csv('BeijingPM20100101_20151231.csv')  
> 此模块的作用是将文件读入DataFrame,还支持可选地将文件迭代或者分割成块。个人觉得是将csv文件加载入pandas,使其具有各种属性，更容易地被编辑和操作。具体文档参考  http://pandas.pydata.org/pandas-docs/version/0.18.1/generated/pandas.read_csv.html

11.python当中的字符串类型的"15"和整数型的15有区别吗？
> 字符串类型的‘15’并不适用所有运算符，而且运算结果仅仅是连接两个字符串，不具有数学含义

12.python的条件语句应该用"=="还是"="？
> Python条件语句是使用if else来表示，变量设定初始值时是用“=”，在判断条件时用“==”给变量赋值。

```python                                                         
eg: name='R'                                  
if name=='python':	                  
	print 'T'                                       
else:  
	print 'F'
```

13.python怎么显示出Hello
> print("Hello")

14.为什么我们从Python开始学习数据分析
> 1、Python 的语法简单，代码可读性高，容易入门，有利于初学者学习。   
> 2、Python 在数据分析和交互、探索性计算以及数据可视化等方面都有非常成熟的库和工具，也有对应的非常活跃的社区。尤其是 Python 中的 Pandas 库在处理中型数据方面可以说有着无与伦比的优势，正在成为各行业数据处理任务的首选库。   
> 3、Python 拥有强大的通用编程能力。Python 不仅在数据分析方面能力强大，在爬虫、web、自动化运维甚至游戏等等很多领域都有广泛的应用。这就使公司使用一种技术完成全部服务成为可能，有利于各个技术组之间的业务融合。   
> 4、Python 是人工智能时代的通用语言。

15.什么是定类变量
> 定类变量是变量的一种，根据定性的原则区分总体和个案类别的变量。定类变量的值只能把研究对象分类，即也只能决定研究对象的同类或不同类