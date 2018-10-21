1.pandas新建一个dataframe可以传入一个字典，比如`dic={'a':1, 'b':0}`,` df=pd.DataFrame(dic)`，除此以外你知道还可以传入什么样的类型和结构构建一个dataframe？

> 除使用包含列表的字典外，还能使用 1.嵌套字典：外层字典的键作为列索引，内层字典的键作为行索引  2.包含series的字典

2.pandas的loc和iloc用法的区别是什么？

> 1. loc——通过行标签索引行数据
>   1.2 loc[‘d’]表示索引的是第’d行（index 是字符）
>   1.3 如果想索引列数据，会报错
>   1.4 loc可以获取多行数据
>   1.5 loc扩展——索引某行某列
>   1.6 loc扩展——索引某列
>
> 2. iloc——通过行号获取行数据
>   2.1 想要获取哪一行就输入该行数字
>   2.2 通过行标签索引会报错
>   2.3 同样通过行号可以索引多行
>   2.4 iloc索引列数据

3.numpy如何生成随机的整数？（参考np.random模块底下的一个方法）

> 用np.random.randint()

4.现在有个类       

```python
class MyClass:                
    variable = "blah"               
    def function(self):                           
        print("This is a message inside the class.")   
```

​      如果我打印MyClass.variable会返回什么？调用MyClass().function()呢？

> print(MyClass.variable)返回结果 blah，print(MyClass().function())返回结果This is a message inside the class.
> None

5.两个集合可能有哪几种运算？（提示：A交B）

> 有4种, 并, 交, 查, 堆成差.
> 给定集合A，B，定义运算∪如下：A∪B = {e|e∈A 或 e∈B}。A∪B称为A和B的并集。
> 给定集合A，B，定义运算∩如下：A∩B = {e|e∈A 且 e∈B}。A∩B称为A和B的交集。
> 给定集合A，B，定义运算-如下：A - B = {e|e∈A 且 e {不属于B}。A - B称为B对于A的差集，相对补集或相对余集。
> 给定集合A，B，定义对称差运算△如下：A△B = (A-B)∪(B-A)。

6.pandas的left join和right join有什么区别？

> pandas中left join是根据左表中的键值去右表中对应的键连接，生成的result表包含左表所有键值，但右表中独有的键值对应的信息不体现；right join则是反过来了。值得注意的是pandas中的left join和right join不同于sql的leftjoin和rightjoin,也不同于excel中匹配函数，pandas中的leftjoin和rightjoin可以实现一对多匹配。

7.如何判断一个元素是否在列表当中？

> 用in 和 not in语句来判断

8.概率的互斥事件是什么意思？

> 事件A和B的交集为空，A与B就是互斥事件，也叫互不相容事件。即不可能同时发生的事件。

9.如何查看列表中的惟一值的个数

> Set集合里的元素都是唯一的，用list创建一个set，set里面的值就是list里的唯一元素值。然后用len（）计算个数。例如len（set【list】）

10.如何给pandas的dataframe df重新更改列名或者索引？(参考df.columns和df.index)

>
> 更改列名:
> df.rename() 支持两种调用的规范:
>    -- (index=index_mapper,columns=colums_mapper)
>    -- (mapper, axis={'index', 'columns'}, ...)
>
> ```python
> df = pd.DataFrame({"A": [1, 2, 3], "B": [4, 5, 6]})
> df.rename(index=str, columns={"A": "a", "B": "c"})
> ```
>
> 更改索引:
>     只介绍一种方式:
>     DataFrame.rename_axis(mapper, axis=0, copy=True, inplace=False)
>     例子:
>
> ```shell
> In [1]: import pandas as pd
>     df = pd.DataFrame({"A": [1, 2, 3], "B": [4, 5, 6]})
>     df
>      Out[1]: 
>                A  B
>             0  1  4
>             1  2  5
>             2  3  6
> ```
>
> ​    
>
>         In [2]: df.rename_axis({0:3,1:4,2:5})
>         Out[2]: 
>                A  B
>             3  1  4
>             4  2  5
>             5  3  6
>     
>         In [3]: df.rename_axis({"A": "a", "C": "c"},axis=1)
>         Out[3]: 
>                a  B
>             0  1  4
>             1  2  5
>             2  3  6
> 参考文档:https://blog.csdn.net/claroja/article/details/72930594?utm_source=itdadao&utm_medium=referral
>

11.pandas绘图语法有哪两种？(提示：plot.bar和plot(kind='bar '))

> plot方法可以生成Series和DataFrame的线型图，对象的索引将用于绘制X轴，kind='bar' 是垂直柱状图。

12.python的类中init是做什么用的

> 是用来初始化新创建对象的状态，在一个对象被创建以后会立即调用 

13.python中的控制流是什么意思

> 控制流是控制代码执行顺序的语句。
> Python用于流程控制的语句包括if条件语句、for和while循环语句、break和continue语句、列表推导（list comprehension）。

14.python中的代码如果要在中途换行怎么办

> 在行末加\

15.python中的matplot库是干什么的

> 用来对数据可视化的