---
title: "List"
permalink: /programming/list/
excerpt: "some notes of learning list"
---

# 两种写法：

```python
range(stop)

range(start, stop[, step])
```

This is a versatile function to create lists containing arithmetic progressions. It is most often used in for loops. The arguments must be plain integers. If the step argument is omitted, it defaults to 1. If the start argument is omitted, it defaults to 0. The full form returns a list of plain integers [start, start + step, start + 2 * step, ...]. If step is positive, the last element is the largest start + i * step less than stop; if step is negative, the last element is the smallest start + i * step greater than stop. step must not be zero (or else ValueError is raised). Example:

```python
>>> range(10)
[0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
>>> range(1, 11)
[1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
>>> range(0, 30, 5)
[0, 5, 10, 15, 20, 25]
>>> range(0, 10, 3)
[0, 3, 6, 9]
>>> range(0, -10, -1)
[0, -1, -2, -3, -4, -5, -6, -7, -8, -9]
>>> range(0)
[]
>>> range(1, 0)
[]
```

## 将elements赋值为range(0,6),而无需使用for循环?

``` python
for i in range(0,6):
	print "Adding %d to the list." %i
	elements.append(i)
```                                              
                     
可以改为：

``` python
elements = range(0,6)                             
```                                                               

## List的其他用法
- [python doc Data Structures](https://docs.python.org/3/tutorial/datastructures.html)

- [Tutorialspoint](http://www.tutorialspoint.com/python/python_lists.htm)

- [RUNOOB 中文](http://www.runoob.com/python/python-lists.html)

``` python
list2 = [1, 2, 3, 4, 5, 6, 7 ];

print "list2[1:5]: ", list2[1:5]
```
输出结果：

```
list2[1:5]:  [2, 3, 4, 5]
```

