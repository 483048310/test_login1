python

序列：相当应一个集合，列表，就是他存的内容

一个可以存储很多东西的，有顺序的存储，可以通过索引去寻找想要的东西

# 索引：

从0开始，左到右

负数开始，右到左，-1开始

```
str="HelloWorld"
print(str[0],"==",str[-10])
print(str[9],"==",str[-1]) 
输出： 
H == H
d == d
```

# 序列相加，

同类型下，

列表只能相加列表

集合和字典不能被索引和相加

```
a=('元组',11,2.2,'abc',True)
b=('元组2',11,2.2,'abc',True)
c='字符串'
都是同类型元组，才能输出，不然报错
```

# 序列相乘

#### 乘多少就打印多少个

集合和字典不能相乘

```
str="HelloWorld"
print(str*3)
输出：HelloWorldHelloWorldHelloWorld
```

# 切片：

切片就是用来截取字符串中一部分内容，然后组成新的字符串

变量名[包括位置，不包括位置,距离多长]

集合和字典不能使用切片

```
str="HelloWorld"
print(str[0:2])#输出0-1的索引，不包括末尾
2Heprint(str[:])#输出全部，一个冒号HelloWorldprint(str[0:10:2])#跳一位输出结果Hlool
```

# 字符串查找

#### 检查元素是否存在序列中

print(查询的元素  in   变量名 )

​				存在就ture，否false

```
str="www.qinjl.com"
print('c'in str)
#输出：True
```

#### 查找对应字符的索引

变量名find（'字符串'）

找不到返回-1



#### 替换字符：

接收变量名=变量名.replace（旧，替换新的）



#### 重复字符：

变量名.count（字符）

#### 改字母大写：

变量名.lower（）



#### 改字母小写：

变量名.upper（）

#### 字母反转：

变量名.swapcase（）



#### 清除空格

左  变量名.lstrip()

右	变量名.rstrip()

全部	变量名.strip()



#### 拆分字符串成列表

变量名.split（'这里位置分隔'）

```
str="www.qinjl.com"
print(str.split('.'))
#['www', 'qinjl', 'com']
```



# 内置函数：

print（）输出

del （变量名）删除

len（）打印他的长度

max（）最大值

id（）返回存储位置

# enumerate（）遍历索引和值

```
for  2/1值 in enumerate(变量名):
1个值返回索引和值
2个返回索引和值
```

range()

​			类型就是range

range（包括位置，不包括位置，步长）

# 转换类型

str（）字符串

list（）列表

set（）集合

tuple()元组

dict()字典

int（）整数

float（）浮点型

bool（）布尔类型





# 转义字符串

#### \n 换行

#### \t 空格



# 字符串格式化

#### \s  字符串

#### \d  整数

#### %%输出%后面的值

# 运算符：

#### 算术运算符，

+-*/%

#### 赋值运算符，

=，+=，a+=b，a=a+b

#### 比较运算符，

==，>= < ,!=

#### 逻辑运算符, 

and ，都要成立才true

or，其中一个成立就成立

not 非

#### 运算符优先级：

# 列表：list[]

列表可以增删改查；可以存放 任何类型的元素

#### 增加

不能直接输入在print输出，也不能用变量=追加

变量名.append（'默认最后那个后面添加进去'）

变量名.extend（如果是序列侧拆分进去，字符串也拆分）

变量名.insert（指定索引，内容）

#### 删除

del   变量名 （指定索引

变量名.pop（指定索引），默认最后

变量名.remover(指定值)

#### 修改：

变量名[索引]='新修改内容'

#### 查询:

升序查询：变量名.sort（）

倒叙查询：变量名.sort（reverse=1）

索引查询相对应值位置：变量名.index(值,从哪个索引开始)

颠倒查询：  变量名.reverse（）

统计相同数量：变量名.count（值）

# 元组()tplue：

 *创建一个元素的元组时，必须带有逗号* tlue(1,)

可以存放任何类型的元素

不能修改

# 字典{}dict

字典里面只能存储键和值的字典，其他类型不能

有键和值，不能索引相加相乘切片，dict{1：'111'}

键是唯一的

要输出两个值

```
set1={1:'123',2:'456',3:'789'}#集合是个无序的
for i in set1:
print(i,set1[i])
```

#### 增加和修改

变量名[索引]=值

#### 删除：

del 变量名 [指定键]

#### items函数：

输出键和值，一个变量，输出两个

for  量1，量2 in  名.items



# 集合set{}

返回无序的随机集合，不会有重复值，不能修改

空集合创建：set1=set（）

#### 添加：

添加单个数据

变量名.app()

添加序列：

update（【1，只能添加序列】，不能单个）

#### 删除：

pop（不能有值）随机删除

​			remove(值)指定删除

​            discard（值）指定数据，如果不存在不会报错



# for循环：

#### 遍历出所有元素

for   自定义名  in    要循环的内容

#### 遍历索引和值

```
for  2/1值 in enumerate(变量名):
1个值返回索引和值
2个返回索引和值
```

#### 双for循环

里面for重新从头循环

#### 遍历字典的键和值：

```python
字典名 = {'1': '键1','键2':'值2'}
for 键,值 in 字典名.items():
    print(key,value)
```

# while循环

条件成立死循环



# if判断：

#### 字符是否存在

if  字符  in    变量名：



#### 是否都是数字：

变量名.isdigit（）

是true，否false

#### 是否都是英文：

变量名.isalpha（）

#### 查找对应字符的索引

变量名find（'字符串'）

#### 字符串转换数字

print（eval('字符串')）

# 列表推导式：

 列表推导式是通过一个可迭代对象来生成列表的 

可以有多个for

a=[（第一个变量，第二个变量名）for (变量名) in  数据  if条件  for。。。。]

变量可以乘除加减

```
# in后面跟其他可迭代对象,如字符串
list_c = [3 * c for c in "python" if条件]
结果['ppp', 'yyy', 'ttt', 'hhh', 'ooo', 'nnn']
```

```
自定义=[[后执行这个] for先执行这个]
list_g = [[x for x in range(g - 3, g)] for g in range(22) if g % 3 == 0 and g != 0]
print(list_g)
结果[[0, 1, 2], [3, 4, 5], [6, 7, 8], [9, 10, 11], [12, 13, 14], [15, 16, 17], [18, 19, 20]]
```



# range函数：

（0，数量-1）

多了遍历会报错

# 函数：

- 封装代码，提高代码重复使用

函数里面调用函数

#### 调用函数：

函数名（实参）

#### 形参

已经定义好的函数，不应该修改里面的代码

可以通过参数

形参函数名（形参）形参是未知数

#### 实参

函数名（实参）

#### 变参：

元组

*代表不定义步长（元组tuple）

def 变量名（*args）

变量（1，2，3）



字典：

def 变量名（键值kwargs）

def 变量名（**kwargs）

变量名（键=值1，键2=值2）

#### 函数嵌套：

一个函数调用另一个函数



#### 局部变量转全局：

global  变量

变量=值

# 类：

 创建对象：对象名1 = 类名() 

class 名 （）：

​		函数=方法

​		变量；

调用  名（）

```python
class num1 ():
    num3='变量'
    def __init__(self):        			self.name='实例化'
    def num2(self):       				print(self.name)
a=num1()第一步调用类
a.num2()第二布调用用的方法
```

#### 普通方法：

def  --init--（self）：

可以直接在类传统参数

def  -- _del_ -- （self）

自动默认最后调用方法

#### 类方法

@classmethod

def    名（cls）

**调用属性：**

cls  属性名

```
class a():

@classmethod
def na(cls):
# cls.name=name
print('输出')

def int1(self):
self.na() 
print('你调用了我')

a=a()
a.int1()
```

**普通方法调用类方法**

类名.方法名（）不用print输出





#### 静态方法：

@staticmethod

def 名（）



#### 封装：

私有化

def  _ _名 () #两条横线

不能调用私有self._ _名值



def  名（）

也不能调用方法_ _名（）

可以调用self.__名值

```python
class num1 ():
  def __in1(self):不能调用self.__名       	self.name='实例化'
  def num2(self):        				不能调用方法def_ _名
    	不能调用self_ _名值
a=num1()
a.num2()
```

#### 继承：

def A(B)A继承B

#### 多个继承：

孙父爷，

输出孙，其他孙.方法输出

#### 属性：

在类里面直接赋值的变量

调用属性

print（类名.属性）

修改属性

类名.属性='修改值'

#### 多态：

 **子类和父类存在相同方法时，子类会覆盖父类方法** 







# exl表格

1.创建表格文件，

2.创建页名

3.在页里面创建表格（几行，几列，内容）

#### 创建表格：

import xlwt

A=xlwt.Workbook('文件名')#在当前目录下创建文件

名=boo.add_sheet(页名')#sheel页命名
booname.write(9,9,'python')#在页里面创建表格索引0开始。内容为

pythonboo.save('文件名)#保存文件

```python
import xlwt
boo=xlwt.Workbook('.\\526.xls')#在当前目录下创建文件booname=boo.add_sheet('sheed')#sheel页命名
booname.write(9,9,'python')#在页里面创建表格索引0开始。内容为pythonboo.save('.\\526.xls')#保存文件
```



#### 查询表格：

xlrd

1.打开文件表格

2.通过索引读取------通过页读取

\，\，读取本地文件的

/读取表格，相对路径

```python
exel = xlrd.open_workbook('.\\5.26.xls')# 读取表格，绝对路径
exel = xlrd.open_workbook('5.26.xls')# 读取表格，相对路径
exel = xlrd.open_workbook('/5.26.xls')# 读取表格，相对路径

table1 = exel.sheet_names()  # 获取表格所有内容
table1 = exel.sheet_by_index(0)  # 通过索引读取表格内容
table2 = exel.sheet_by_name('sheed')  # 通过页名读取# 

通过（y,x）索引值,（加.value少number:）
print(table1.cell(3, 2))  # （y,x）也是通过索引读取
print(table2.cell(3, 2).value)  # （y,x）也是通过索引读取

#取得有效无效行和列
maxrows=sheet1.nrows
maxcols=sheet1.ncols
print("有效的行=%d，列=%d"%(maxrows,maxcols))

打印他有多少行多少列
```



# 接口请求

1.导入import  request请求包



2.发送请求

登录需要携带data，转换json格式

参数是网址后面的参数

A=request.ge/post(地址，数据data，参数parmes)



3，打印看看成功

6

1