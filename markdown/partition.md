---
name: partition
video-id: 730823116
---

Splits the list into two parts. The first part contains all the elements that satisfy the predicate, and the second part contains those that do not.

# SIGNATURE
```scala
def partition(p: A => Boolean): (List[A], List[A])
```

# EXAMPLE
```scala
val list = List(1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
val (evens, odds) = list.partition(_ % 2 == 0)
---
evens = List(2, 4, 6, 8, 10)
 odds = List(1, 3, 5, 7, 9)
```