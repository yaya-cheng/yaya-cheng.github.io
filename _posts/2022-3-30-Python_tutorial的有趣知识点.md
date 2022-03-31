---
layout: post
title:  "桂桂卷的入职准备-python学习"
header-img: "img/桂桂狗3-dimm.jpg"
categories: Onboarding Preparation
tags: Work hard(๑･`◡´･๑)
author: CYY
---

💗入职前的草莓桂桂卷(๑•̀ㅂ•́)و✧
{% raw %}

![image](/img/split-line1.gif)
### 4.8.1-Default Argument Values

#### 🍓Example 1

Important warning: The default value is evaluated only once. This makes a difference when the default is a mutable object such as a list, dictionary, or instances of most classes. For example, the following function accumulates the arguments passed to it on subsequent calls:

```python
def f(a, L=[]):
    L.append(a)
    return L

print(f(1))
print(f(2)) 
print(f(3))
```

输出
```python
[1]
[1, 2]
[1, 2, 3]
```
If you don’t want the default to be shared between subsequent calls, you can write the function like this instead:
```python
def f(a, L=None):
    if L is None:
        L = []
    L.append(a)
    return L
```
见[这里](https://docs.python.org/3/tutorial/controlflow.html)

{%endraw%}


