---
title: Lists in Python
categories:
  - Sports
  - Baseball
date: 2017-12-01 18:57:52
tags:
---

Lists can be used to store multiple elements of the same or different datatypes. Lists are variable length data structure. If you are new you will be using this a lot and if you have been using it, let me share some more tips and tricks.

{% codeblock lang:py %}
abc = list()
{% endcodeblock %}

`abc.append()` Adds at the end of the list. Time Complexity O(1)

{% codeblock %}
abc.append('a')
print abc
['a']
abc.append('b')
['a', 'b']
{% endcodeblock %}

Similar methods for adding to a list are `.insert(index, elem)` & `.extend(another_list)`

`.insert(index, elem)` inserts the element at the given index, shifting elements to the right. Time Complexity O(n).

`abc.extend(def)` adds the elements in list `def` to the end of the list `abc`. Time Complexity O(k), where k is the length of list `def`

{% codeblock %}
def = list()
def.append('d')
print def
['d']
def.append('e')
['d', 'e']
abc.extend(def)
print abc
['a', 'b', 'd', 'e']
{% endcodeblock %}

