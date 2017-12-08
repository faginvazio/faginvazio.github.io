---
layout: post
title:  "Variables and Data types"
date:   2017-12-09 12:26 +1100
categories: python variable datatype
---
Hi, Today I explain python variable and data types.

Variables look like this.
`nami`, `Nami`, `nami23`, `_name`, ...

They are used to store references to the values in memory.
As you can see you can use letters, digits, and underscores.
You cannot start with digit.
You cannot use any reserved words, aka keywords like `and`, `if`, `for`, `True`, ...

  [**python keywords**][python keywords]
  ```   
  False      class      finally    is         return
  None       continue   for        lambda     try
  True       def        from       nonlocal   while
  and        del        global     not        with
  as         elif       if         or         yield
  assert     else       import     pass
  break      except     in         raise
  ```

Don't worry about memorising all reserved words.
If you try to use them, you get a SyntaxError.

  ```python3
  >>> if = nami
    File "<stdin>", line 1
      if = nami
         ^
  SyntaxError: invalid syntax
  >>>
  ```

Lets talk about basic python data types.
There are `int`, `float`, `str`, `bool`, `list`, `tuple`, `dict`.

You can find out which type it is.
  ```python3
  >>> nami = 23
  >>> type(nami)
  <class 'int'>
  >>>
  >>> nami = 'Nami'
  >>> type(nami)
  <class 'str'>
  >>>
  ```
I think there are so many things we can learn. I'll talk about them as simple as I can.
That's what I'm going to try.

Cheers :beers:

[python keywords]: https://docs.python.org/3.5/reference/lexical_analysis.html
