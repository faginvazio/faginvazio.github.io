---
layout: post
title:  "Basic assignment"
date:   2017-12-16 12:26 +1100
categories: python assignment
---
Hi,
I'm gonna tell 2 things today.
They are `=` (aka, assignment operator), and `values`.

Assignment is assigning a value to a variable.

Some examples:

  ```python
  name = 'nami'
  age = 22
  height = 162.56
  points = [14, 15, 16]
  live = True
  ```

Everything is object in python.
In the above examples, the right-hand side is value, which itself is an object.
The left-hand side is variable. **=** is assignment operator. Assigning a value to a variable means that a variable get reference to value.

You can assign simultaneously like this,

  ```python
  name, age, height = 'nami', 22, 162.56
  ```

This simultaneous assignment is useful to swap values.

  ```python
  name_1, name_2 = 'nami', 'luffy'
  print(name_1, name_2)  ## nami luffy

  name_1, name_2 = name_2, name_1
  print(name_1, name_2)  ## luffy nami
  ```
