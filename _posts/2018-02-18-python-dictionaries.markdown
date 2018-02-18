---
layout: post
title:  "Dictionaries in Python"
date:   2018-02-18 12:26 +1100
categories: python dictionaries
---

Hi,
I'm going to talk about dictionary in python today.
It is used to store key value pairs.
Key must be of hashable type.

### [ hashable ][python glossary]

> An object is hashable if it has a hash value which never changes during its lifetime (it needs a **hash**() method), and can be compared to other objects (it needs an **eq**() method). Hashable objects which compare equal must have the same hash value.
>
> Hashability makes an object usable as a dictionary key and a set member, because these data structures use the hash value internally.
>
> All of Python’s immutable built-in objects are hashable; mutable containers (such as lists or dictionaries) are not. Objects which are instances of user-defined classes are hashable by default. They all compare unequal (except with themselves), and their hash value is derived from their id().

Here are some basic dictionary examples.

```python
myDictPairs = {}
myFriendsNameAndBounty = {
    'luffy': 30,
    'zoro': 20
}

print(myDictPairs)
print(myFriendsNameAndBounty)
print(myFriendsNameAndBounty['luffy'])

myFriendsNameAndBounty['sanji'] = 15
print('After adding Sanji', myFriendsNameAndBounty)

del myFriendsNameAndBounty['zoro']
print('After Deleting Zoro', myFriendsNameAndBounty)

for key in myFriendsNameAndBounty:
    print(key, myFriendsNameAndBounty[key])

print('The length of myFriendsNameAndBounty', len(myFriendsNameAndBounty))

print('luffy in myFriendsNameAndBounty', 'luffy' in myFriendsNameAndBounty)
print('zoro not in myFriendsNameAndBounty', 'zoro' not in myFriendsNameAndBounty)

print(myFriendsNameAndBounty.keys())

print(myFriendsNameAndBounty.get('luffy'))
print(myFriendsNameAndBounty.get('zoro', 'not my friends'))

print('pop luffy', myFriendsNameAndBounty.pop('luffy'), myFriendsNameAndBounty)

# {}
# {'luffy': 30, 'zoro': 20}
# 30
# After adding Sanji {'luffy': 30, 'zoro': 20, 'sanji': 15}
# After Deleting Zoro {'luffy': 30, 'sanji': 15}
# luffy 30
# sanji 15
# The length of myFriendsNameAndBounty 2
# luffy in myFriendsNameAndBounty True
# zoro not in myFriendsNameAndBounty True
# dict_keys(['luffy', 'sanji'])
# 30
# not my friends
# pop luffy 30 {'sanji': 15}
```

Cheers :beers: :dog:

[python glossary]: https://docs.python.org/3/glossary.html
