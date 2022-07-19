---
name: dropWhile
---

Returns a suffix of the list, dropping elements from the head of the list until the predicate fails.

# SIGNATURE
```scala
def dropWhile(p: A => Boolean): List[A]
```

# EXAMPLE
```scala
val list = List(1, 2, 4, 6, 3, 0, 8, 5)
val rest = list.dropWhile(_ < 5)
---
rest = List(6, 3, 0, 8, 5)
```
