drop

Drops the first `n` elements from the list.

```scala
def drop(n: Int): List[A]
```

```scala
val list = List(1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
val lost = list.drop(3)
---
lost = List(4, 5, 6, 7, 8, 9, 10)
```