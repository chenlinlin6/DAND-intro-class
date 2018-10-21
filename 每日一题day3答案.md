1.这里提示if count=1那一行invalid syntax，‘invalid syntax’中文意思是什么？你认为哪里写错了？

```python
def if_conditions():
	count=1
	if count==1
    	return 'hello'
```

> invalid syntax指语法错误。应写成if count==1 ：，加上：冒号。

2.什么是布尔值？

> Boolean中的True和False是布尔值，主要用于逻辑运算。

3.python当中遍历(loop)是什么意思？

> 遍历的意思就是查看集合中的元素，每次取集合中的一个元素并操作。
> 例子：
>
> ```python
> for v in range(4,8):  
>     print(v)  
> ```
>
> 输出效果如下：
>
> ```python
> 4
> 5
> 6
> 7
> ```
>
> 

4.python代码里面文本注释前面要加什么符号？

> \#

5.python的strip语法是做什么用的？

> Python strip() 方法用于移除字符串头尾指定的字符（默认为空格或换行符）。

6.如何查看dataframe df的列名和索引名字？(提示：列和索引的英文单词)

> df.columns和df.index，可以用这个来对列名和索引名字进行修改。比如df.columns=['a','b','c']

7.请问在判断语句当中and和or有什么区别？

> and，or 和not是三种布尔逻辑运算符。1). x or y表示 if x is false,then y, else x  2).x and y表示 if x is false,then x,  else y  3). and 优先级高于or

8.pandas中的series和dataframe有什么区别？

> Series相当于数组
> DataFrame相当于有表格，有行表头和列表头
> DataFrame可以看作是由一列列Series组成的，如果要这么生成DataFrame的话，需要采用字典模式的参数。Series也可以有index，但没有columns。

9.假设有一列‘PM_US Post ’，df[‘PM_US Post ’].sum()的输出是什么值

> PM_US Post这一列值的和

10.Shanghai_data里面的'season'这一列是1,2,3,4的取值，请问Shanghai_data['season'] = Shanghai_data['season'].map({1:'Spring', 2:'Summer', 3:'Autumn', 4: 'Winter'})这里的map方法做了什么事情？

> Shanghai_data中season列中的值是1,2,3,4.但是我们不知道1,2,3,4所代表的具体含义。通过map()函数加入一个字典，将season列中的1,2,3,4映射到Spring,Summer,Autumn,Winter.从而将1,2,3,4具体转换为字符串Spring,Summer,Autumn,Winter.

11.pandas的dataframe有很多方法的参数都有axis这一项，比如dropna，sum等，axis可以为1或者0。你是如何理解axis=1和axis=0的？（提示：从列和行的方向考虑）

> 使用0值表示沿着每一列或行标签向下执行方法，使用1值表示沿着每一行或者列标签模向执行对应的方法。

12.python当中整数和浮点数的计算是一样的吗？比如`6/7`返回的结果是什么？如果我想要返回有小数位数的浮点数，应该怎么写？(提示：把分子或者分母变成浮点数)

> ```python
> print （6/7） 
> >>>0.85714285714857142 ; 
> print ('%.2f'%(6/7)) 
> >>>0.86
> ```

13.df_all_cities.head(10)会显示几行数据

> 10行

14.info()是干什么用的

> info函数可以看到数据的信息，比如总的数量，有多少是空的，等等

15.csv文件和tsv文件的区别

> csv为用逗号分隔的文本文件，tsv为用制表符tab分隔的文本文件

