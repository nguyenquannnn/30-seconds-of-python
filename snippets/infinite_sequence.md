---
title: infinite_sequence
tags: utility, function, intermediate
---

Using a generator, lazily generate a sequence of infinite number.

- Initialize `num` at 0
- While looping an infinite loop, yield `num` and return its value
- Increment `num` by 1 

```py
def infinite_sequence():
  num = 0
  while True:
    yield num
    num += 1
```

```py
for i in infinite_sequence():
  print(i, end=" ")
# 1 2 3 4 5 6 ... 950434 950435
```
