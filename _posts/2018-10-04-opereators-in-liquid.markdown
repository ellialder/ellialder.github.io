---
layout: post
title: Operators in Liquid
date: 2018-10-04 13:32:20 +0300
description: operators in liquid
img: liquid-markdown.jpg # Add image post (optional)
tags: [liquid]
---
Liquid bao gồm nhiều toán tử logic và so sánh.
# Basic

|Toán tử | Ý nghĩa               |                              
| --- | ------------------------ |
| ==  | equals                   |
| !=  | does not equal           |
| >   | greater than             |
| <   | less than                |
| >=  | greater than or equal to |
| <=  | less than or equal to    |
| or  | logical or               |
| and | logical and              |

For example:

```
{% if product.title == "Awesome Shoes" %}
  These shoes are awesome!
{% endif %}
```

> Bạn có thể sử dụng nhiều toán tử trong tag:

```
> {% if product.type == "Shirt" or product.type == "Shoes" %}
  This is a shirt or a pair of shoes.
{% endif %}
```

### Contain
`contain` chứa các kiểm tra cho sự hiện diện của một chuỗi con bên trong một chuỗi.

```
{% if product.tags contains 'Hello' %}
  This product has been tagged with 'Hello'.
{% endif %}
```
`contain` có thể tìm kiếm chuỗi. Bạn không thể sử dụng nó để kiểm tra một đối tượng trong một mảng các đối tượng.


