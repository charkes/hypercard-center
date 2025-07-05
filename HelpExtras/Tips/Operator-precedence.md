---
title: Operator precedence
card_id: 8338
---

### Operator precedence

Each operator has an order of precedence. Use the chart below as a guide. HyperCard evaluates operators with lower order numbers before those with higher order numbers. Operators with the same order number are evaluated in an expression from left to right. 

```
Order   Operators
1      ()
2      - [minus sign]
       not
       there is a
       there is an
       there is not a
       there is not an
       there is no
3      ^
4      * / div mod
5      + -
6      & &&
7      < > <= >= ≤ ≥
       is in
       contains
       is not in
       is a
       is an
       is not a
       is not an
       is within
       is not within
8      = is
       is not <> ≠
9      and
10      or
```

Use parentheses to eliminate ambiguity in the process of evaluation—parentheses have the highest order of precedence:` (3+2) * 5 = 25`. If you use parentheses, HyperCard evaluates the innermost parenthetical expression first. 