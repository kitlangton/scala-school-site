---
name: partition
video-id: 730823116
---

Returns a tuple of two new lists. The first list consists of the elements that satisfy the predicate. The second list 
consists of those that do not.

# SIGNATURE
```scala
def partition(p: A => Boolean): (List[A], List[A])
```

# EXAMPLE
```scala
val list = List(1, 2, 3, 4, 5, 6, 7, 8)
val (evens, odds) = list.partition(_ % 2 == 0)
---
evens = List(2, 4, 6, 8)
 odds = List(1, 3, 5, 7)
```