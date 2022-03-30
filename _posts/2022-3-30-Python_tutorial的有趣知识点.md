---
layout: post
title:  "桂桂卷的入职准备-python学习"
header-img: "img/桂桂狗3-dimm.jpg"
categories: Onboarding Preparation
tags: Work hard(๑･`◡´･๑)
author: CYY
---

入职前的草莓桂桂卷(๑•̀ㅂ•́)و✧
{% raw %}

### 题目描述

给定单向链表的头指针和一个要删除的节点的值，定义一个函数删除该节点。返回删除后的链表的头节点。注意：此题对比原题有改动

示例 1:

输入: head = [4,5,1,9], val = 5

输出: [4,1,9]

解释: 给定你链表中值为 5 的第二个节点，那么在调用了你的函数之后，该链表应变为 4 -> 1 -> 9.


示例 2:

输入: head = [4,5,1,9], val = 1

输出: [4,5,9]

解释: 给定你链表中值为 1 的第三个节点，那么在调用了你的函数之后，该链表应变为 4 -> 5 -> 9.

### 单指针python版

```python
# Definition for singly-linked list.
# class ListNode:
#     def __init__(self, x):
#         self.val = x
#         self.next = None
class Solution:
    def deleteNode(self, head: ListNode, val: int) -> ListNode:
        pre=head
        if head.val==val: return head.next
        while(pre.next.val!=val):
            pre=pre.next
        pre.next=pre.next.next
        return head
```

最近成都实在是太热啦，本桂桂酱刚刚吃了一颗冰淇凌嘻嘻，你们呐？

最近天热，要注意不要中暑了嗷˶´⚰︎`˵

![image](/img/剑指18配图.jpg)

{%endraw%}


