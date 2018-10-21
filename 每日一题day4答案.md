1.while循环中break和continue是什么意思？

> continue 用于跳过该次循环，break 则是用于退出循环。

2.列表怎么样进行排序？

> 使用.sort（）方法进行排序，其中reverse = True 是降序， reverse = False 是升序（默认）。

3.列表如何追加元素，比如有个列表li=[1,2,3]，我怎么往里面加个字符串'a'？

> li.append('a')

4.`[i.upper() for i in ['a', 'b', 'c']]`返回的结果是什么？你如何描述中间执行的过程？

> 返回的结果是：['A', 'B', 'C']。upper（）是将对象全部大写，这个语句可以理解为大写当i为a,b,c

5.尝试运行下`['a']*10`，返回什么？

>  ['a', 'a', 'a', 'a', 'a', 'a', 'a', 'a', 'a', 'a']

6.项目当中有很多方法里面都有符号"."，比如`city_data.head()`，比如`data.groupby(key)['PM_US Post'].mean().plot(kind = 'bar', color = color)`，这个符号代表着"`.`"前后的对象和属性或者方法的什么关系（提示：面向对象编程，类似于超市这个对象有收银台，生鲜区等属性）

> 抽象与具体的关系。例如A.B表示A对象的B属性（或A属性的B方法）

7.python的类是什么东西？类和类的对象是什么关系（提示：参照超市与沃尔玛，家乐福以及乐天的关系）

> 类是用来描述具有相同的属性和方法的对象的集合。它定义了该集合中每个对象所共有的属性和方法。对象是类的实例。 超市好比是‘类‘，家乐福沃尔玛好比‘对象’。

8.在计算中位数的时候，异常对结果的影响大不大？

> 影响不大  中位数的优势在于它能避免数据的平均水平受到异常值的影响。

9.python 中的 `def` 是干什么用的

> def是define的意思，在python中用来定义函数。例如
> 定义函数
>
> ```python
> def hello():
>   print("hello")
> #调用函数
> hello（）
> ```

10.`if a = b：`这行代码是干什么的，有没有什么问题

> =是赋值符号，表示将右边的值赋予左边变量。if 后应该接一个布尔值。应改为 if a==b:

11.`a = [], b = (), c = {}`     请问这3个有什么区别

> Python中的小括号（）：代表tuple元祖数据类型，元祖是一种不可变序列。Python中的中括号[]：代表list列表数据类型，列表是一种可变序列。Python中的花括号{}：代表dict字典数据类型，字典是Python中唯一内建的映射类型。

12.pandas删除缺失值用什么方法？是在原本的dataframe上面修改的吗？

> 删除含有空缺值的行：data=data.dropna()
> 删除全为NaN的行：data=data.dropna(how='all')
> 删除全为NaN的列：data=data.dropna(axis=1,how='all')，在原来的dataframe上做修改之后返回一个新的dataframe

13.如何查看一个dataframe里面有多少条数据？

> 采用函数DataFrame.describe()可以查看关于数值字段的统计学数值，包括中位数，分位数，平均值，标准偏差等等。用len(df)可以查看dataframe的数据数目

14.我们做项目的jupyter notebook是干什么程序。

> 是用来实现代码运行，解释文字说明和可视化的一个编辑器

15.jupyter notebook中使用的markdown记录框。markdown是什么？

> Markdown是格式化语法，可让你加入链接、将文本样式设为粗体或斜体和设置代码格式。

