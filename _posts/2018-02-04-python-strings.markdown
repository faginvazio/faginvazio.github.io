---
layout: post
title:  "Strings in Python"
date:   2018-02-04 12:26 +1100
categories: python strings
---
Hi,
Today I'm going to talk about strings.
I don't want to describe all functions related strings.
Just interesting ones for me. :tongue:
I'm sure you can get it if you read the code.


  ```python
  name = "Nami"
  empty_string = str()
  greeting = "Hi"
  white_space = "\t"
  luffy = "\"nami, you're always my friend.\""

  print("2 times name + empty_string + 3 times greeting is: ",
    name * 2 + empty_string + greeting * 3)
  print("The length of the name: ", len(name))
  print("zo in Nami is ", "zo" in name)
  print("am in Nami is not ", "zo" in name)
  print("Nami is alphanumeric: ", name.isalnum())
  print("Nami is alphabets only: ", name.isalpha())
  print("Nami is digits only: ", name.isdigit())
  print("white_space is only whitespace: ", white_space.isspace())
  print(luffy, " is ends with end.: ", luffy.endswith("end."))
  print(luffy, " is ends with end.\": ", luffy.endswith("end.\""))
  print(luffy, " is starts with \"nam: ", luffy.startswith("\"nam"))
  print(luffy, " has count of 'a': ", luffy.count("a"))
  print(luffy.title())
  print(luffy.upper())
  print(luffy.upper().lower())
  print(luffy.replace("always", "not"))
  print("luffy[:] = ", luffy[:])
  print("luffy[:9] = ", luffy[:9])
  print("luffy[4:] = ", luffy[4:])
  print("luffy[4:9] = ", luffy[4:9])
  print("luffy[1:-1] = ", luffy[1:-1])

  # 2 times name + empty_string + 3 times greeting is:  NamiNamiHiHiHi
  # The length of the name:  4
  # zo in Nami is  False
  # am in Nami is not  False
  # Nami is alphanumeric:  True
  # Nami is alphabets only:  True
  # Nami is digits only:  False
  # white_space is only whitespace:  True
  # "nami, you're always my friend."  is ends with end.:  False
  # "nami, you're always my friend."  is ends with end.":  True
  # "nami, you're always my friend."  is starts with "nam:  True
  # "nami, you're always my friend."  has count of 'a':  3
  # "Nami, You'Re Always My Friend."
  # "NAMI, YOU'RE ALWAYS MY FRIEND."
  # "nami, you're always my friend."
  # "nami, you're not my friend."
  # luffy[:] =  "nami, you're always my friend."
  # luffy[:9] =  "nami, yo
  # luffy[4:] =  i, you're always my friend."
  # luffy[4:9] =  i, yo
  # luffy[1:-1] =  nami, you're always my friend.

  ```






Cheers :beers:
