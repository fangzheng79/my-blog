---
title: 2 Tricks of Python Dictionary
date: 2020-07-09
img: ./python_dic.png
tags: [Python]
---
最近用到的python字典的两个trick，mark一下。

## python字典(dict)相加，相同key相加，不同key保留

假如 两个字典dict1={'a':1,'b':2,'c':3},dict2={'c':4,'d':5}，若两个dict1和dict2有相同的key则对应的value相加，若没有则直接添加过来。结果为dict3={'a':1,'b':2,'c':7,'d':5}

```python
def merge_dict(x,y):
    for k,v in x.items():
                if k in y.keys():
                    y[k] += v
                else:
                    y[k] = v
```

底下这个是所有元素相加

```python
x={'a':1,'b':2,'c':3}
y={'c':4,'d':5}
from collections import Counter
X,Y=Counter(x),Counter(y)
z=dict(X+Y)
print(z)
```

## python中按value取字典中前n个最大或最小值

python中的字典是无序的，但是有时候会根据value值来取得字典中前n个值，本文思想是将字典转化成list，经过排序，取得前n个值，再将list转化回字典，代码如下：

```python
n = 2 
a = {'a':9,'b':1,'c':5}

L = sorted(a.items(),key=lambda item:item[1],reverse=True)
L = L[:n]
print(L)
 
dictdata = {}
for l in L:
    dictdata[l[0]] = l[1]
 
print (dictdata)
```