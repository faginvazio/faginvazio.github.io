---
layout: post
title:  "Lists in Python"
date:   2018-02-11 12:26 +1100
categories: python lists
---

Hi,
Today is List day. So lets celebratge it. :cake:
I think it's important to keep in mind that **lists are mutable**.
I'm going to just show some simple examples. It's basic.

```python
myRepsList = [1001, 1002, 1003, 1004]
myFriendsList = ['Luffy', 'Zoro', 'Sanji']
myMixedList = [100, 'berry', 'storm', [1, 2, 3], True]
myEmptyList = []
myEmptyList2 = list()
myComprehensionList = [x for x in range(10)]

print(myRepsList[0])
print(myFriendsList[1])
print(myMixedList)
print(myEmptyList)
print(myEmptyList2)
print(myComprehensionList)
print('Ray is in myFriendsList: ', 'Ray' in myFriendsList)
print('Usopp is not in myMixedList: ', 'Usopp' not in myMixedList)

myConcatList = myRepsList + myMixedList
print('myRepsList + myMixedList: ', myConcatList)
print('length of myConcatList: ', len(myConcatList))

mySlicedList = myConcatList[1:4]
print('new index from index 1 to 4 (including 1, excluding 4): ', mySlicedList)

for i in mySlicedList:
    print(i)

print(
    'Append Chopper to myFriendsList: it returns',
    myFriendsList.append('Chopper'),
    '\t The myFriendsList: ',
    myFriendsList
    )

print(
    'Append all elemnents in the myRepsList to myComprehensionList: it returns',
    myComprehensionList.extend(myRepsList),
    '\t The myComprehensionList: ',
    myComprehensionList
    )

print(
    'Insert 1000 into index  0: it returns',
    myRepsList.insert(0, 1000),
    '\t The myRepsList: ',
    myRepsList
    )

print(
    'It returns the index of the first occurrence of element in myMixedList: ',
    myMixedList.index('storm')
    )

print(
    'It remove the first occurence of element in myFriendsList: it returns',
    myFriendsList.remove('Zoro'),
    '\t The myFriendsList: ',
    myFriendsList
    )

print(
    'Reverse myFriendsList: it returns',
    myFriendsList.reverse(),
    '\t The myFriendsList: ',
    myFriendsList
    )

print(
    'Sorting myFriendsList: it returns',
    myFriendsList.sort(),
    '\t The myFriendsList: ',
    myFriendsList
    )

print(
    'Remove the element at the index and return it from myFriendsList',
    myFriendsList.pop(1),
    '\t The myFriendsList: ',
    myFriendsList
    )


# 1001
# Zoro
# [100, 'berry', 'storm', [1, 2, 3], True]
# []
# []
# [0, 1, 2, 3, 4, 5, 6, 7, 8, 9]
# Ray is in myFriendsList:  False
# Usopp is not in myMixedList:  True
# myRepsList + myMixedList:  [1001, 1002, 1003, 1004, 100, 'berry', 'storm', [1, 2, 3], True]
# length of myConcatList:  9
# new index from index 1 to 4 (including 1, excluding 4):  [1002, 1003, 1004]
# 1002
# 1003
# 1004
# Append Chopper to myFriendsList: it returns None 	 The myFriendsList:  ['Luffy', 'Zoro', 'Sanji', 'Chopper']
# Append all elemnents in the myRepsList to myComprehensionList: it returns None 	 The myComprehensionList:  [0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 1001, 1002, 1003, 1004]
# Insert 1000 into index  0: it returns None 	 The myRepsList:  [1000, 1001, 1002, 1003, 1004]
# It returns the index of the first occurrence of element in myMixedList:  2
# It remove the first occurence of element in myFriendsList: it returns None 	 The myFriendsList:  ['Luffy', 'Sanji', 'Chopper']
# Reverse myFriendsList: it returns None 	 The myFriendsList:  ['Chopper', 'Sanji', 'Luffy']
# Sorting myFriendsList: it returns None 	 The myFriendsList:  ['Chopper', 'Luffy', 'Sanji']
# Remove the element at the index and return it from myFriendsList Luffy 	 The myFriendsList:  ['Chopper', 'Sanji']
```

Cheers :beers:
