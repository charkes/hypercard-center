---
title: How HyperTalk sees a line
card_id: 24266
---

### How HyperTalk sees a line

When you use a chunk expression that involves lines, such as

```
line 3 of field "text"
line 1 to 2 of card field 1
```

a return character determines a line, not the line wrap. A line that wraps and is displayed as two lines is seen as one line by HyperTalk. 