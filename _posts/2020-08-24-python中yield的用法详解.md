---
title: python中yield的用法详解
tags: python
---
可以yield看做“return”，普通的return是什么意思，就是在程序中返回某个值，返回之后程序就不再往下运行了

```python
def foo():
    print("starting...")
    while True:
        res = yield 4
        print("res:",res)
g = foo()
print(next(g))
print("*"*20)
print(next(g))
```

