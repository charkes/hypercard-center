---
title: cantPeek
card_id: 69328
---

# cantPeek

```
set [the] cantPeek of [ph:stack] ¬
     to [ph:trueOrFalse]
```

The `cantPeek` property returns or sets whether users can press Command-Option or  Command-Shift-Option to peek at the location of buttons and fields and use the  Command-Option shortcuts for accessing scripts. It corresponds to the Can’t Peek option in the Protect Stack dialog box. 

The default value is `false`, meaning that you <u>can</u> peek at fields and buttons and use the Command-Option shortcuts for accessing (or peeking at) scripts.

## Examples

```
set the cantPeek of this stack to true
set the cantPeek of stack "Home" to true
```
