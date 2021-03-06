# Python中的组等基本概念

Python组的概念

列表(list),是可变的</br>
列表的定义:[1,2,3,4,5,6]</br>
里面可以是字符串,或bool类型,或数字类型等任意的类型</br>
[“hello”,”world”,1,2,True]等

同时,列表里面依然可以是列表</br>
[[1,2],[3,4],[True,False]],可以称之为嵌套列表(二维数组)

可以和字符串一样获取列表中的某一个元素</br>
例如:[1,2,3,4][0]</br>
注意:当后面为数字,[1,2,3,4][0]结果为1</br>
         当后面为冒号形式,[1,2,3,4][-1:]结果为[4]

同样的,字符串的截取和合并方式和字符串一样..</br>
即两个列表可以使用相加和相乘一个数字</br>
但注意,列表没有减这个操作

元组(tuple),是不可变的</br>
元组的定义:(1,2,3,4,5,6)</br>
与列表一致,元组内也可以是任何类型及其组合,与字符串和列表一致,可以通过数字或者冒号的方式访问元组中的元素,同时也可以使用加号或者乘号


当元组元素只有一个元素时,编译器会将()理解为数学运算中的(),即会将1运算出来,即单个元素是什么类型就是什么类型
若一定需要表示单个元素的元组,则可以表示为(1,)(加一个逗号即可)</br>
()则标示一个元素都没有的空元组

str,list,tuple都可以称之为序列</br>
序列的共同点:</br>
序列的每一个元素都有一个序号,及[1,2,3][2].结果为3</br>
切片:[1,2,3][-1:]</br>
序列可以加法和乘法操作</br>
in与not in函数,都是序列共有的</br>
len函数作用为序列内部有几个元素</br>
max函数求序列中的最大元素</br>
min函数求序列中的最小元素</br>
注:使用max函数或者min函数中,若其中为字符串,则结果为字母在字母表中的位置得出结果,即acell码

in函数,是否在…3 in [1,2,3,4,5],答案为True,即结果为True类型

not in函数,是否不在,即3 not in [1,2,3,4,5],答案为False

ord函数可以求出某个字符的acell码

集合(set)  —>无序</br>
{1,2,3,4,5,6}即是一个集合</br>
特点:1.不能使用下标索引和切片操作</br>
         2.不重复,即{1,1,2,2,3,3,4,4}即为{1,2,3,4}</br>
         3.也能使用len,in,not in函数</br>
         4.可以使用”-”运算符,即求两个集合的差集,{1,2,3,4,5,6} - {2,3} 结果为{1,4,5,6}</br>
         5.可以使用”&”运算符,即求两个集合的交集,{1,2,3,4,5,6} &{3,4}记过为{3,4}</br>
         6.可以使用”|”运算符,即求两个集合的并集,{1,2,3,4,5,6} |{3,4,7},结果为{1,2,3,4,5,6,7}

定义一个空的集合:set()

字典(dict),是集合类型,也是无序的</br>
{key1 : value1,key2 : value2}</br>
常用的操作是,通过key,来得到value</br>
{1:’hello’,2:”world”}[1]

注,字典是不能有重复的键,虽然不会报错

value可以使用str,int等任意类型</br>
key必须是不可变的类型,即int,str等,若为列表等可变的元素,会报错</br>
空字典的定义 {}