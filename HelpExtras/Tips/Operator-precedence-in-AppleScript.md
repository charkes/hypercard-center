---
title: Operator precedence in AppleScript
card_id: 54859
---

### Operator precedence in AppleScript

Each operator in AppleScript has an order of precedence. Use the chart below as a guide. AppleScript evaluates operators with lower order numbers before those with higher order numbers. Operators with the same order number are evaluated in an expression from left to right. 

```
Order   Operators
1      ()
2      - [minus sign]
       + [plus sign]
3      ^
4      * / ÷ div mod
5      + - [addition & subtraction]
6      as
7      < > <= >= ≤ ≥
8      =  ≠
9      not
10      and
11      or
```

Use parentheses to eliminate ambiguity in the process of evaluation—parentheses have the highest order of precedence:` (3+2) * 5 = 25`. If you use parentheses, AppleScript evaluates the innermost parenthetical expression first. 