---
name: takeWhile
---

Returns a prefix the list, taking from the head of the list until the predicate fails.

# SIGNATURE
```scala
def takeWhile(p: A => Boolean): List[A]
```

# EXAMPLE
```scala
val list  = List(1, 2, 4, 6, 3, 0, 8, 5)
val start = list.takeWhile(_ < 5)
---
start = List(1, 2, 4)
```
