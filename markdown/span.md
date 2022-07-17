span

Returns two lists; the first takes elements from the head of the list until the predicate fails, and the second contains the rest. A combination of dropWhile and takeWhile.

```scala
def span(p: A => Boolean): (List[A], List[A])
```

```scala
val list = List(1, 2, 3, 4, 5, 6, 7, 8, 9, 10)
val (lessThanFive, greaterThanFive) = list.span(_ < 5)
---
lessThanFive = List(1, 2, 3, 4)
greaterThanFive = List(5, 6, 7, 8, 9, 10)
```
