---
name: span
video-id: 730839597
---

Returns a tuple of two new lists. The first list consists of elements taken from the head of the list until the predicate
fails. The second list consists of the remaining elements.

This is essentially an optimized combination of [takeWhile](#list-method-takeWhile) and [dropWhile](#list-method-dropWhile).

# SIGNATURE
```scala
def span(p: A => Boolean): (List[A], List[A])
```

# EXAMPLE
```scala
val list = List(1, 2, 3, 4, 5, 6, 5, 4, 3, 2, 1)
val (start, rest) = list.span(_ < 5)
---
start = List(1, 2, 3, 4)
 rest = List(5, 6, 5, 4, 3, 2, 1)
```

# EQUAL TO
```scala
val (start, rest) = (list.takeWhile(_ < 5), list.dropWhile(_ < 5))
```