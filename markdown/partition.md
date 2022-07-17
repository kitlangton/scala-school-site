partition

Returns two lists; the first containing elements that satisfy that predicate, and the second containing the rest.

It's all very cool!

```scala
def partition(p: A => Boolean): (List[A], List[A])
```

```scala
val list = List(1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
val (evens, odds) = list.partition(_ % 2 == 0)
---
evens = List(2, 4, 6, 8, 10)
odds = List(1, 3, 5, 7, 9)
```
