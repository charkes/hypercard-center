---
title: Don’t use “the” with format names
card_id: 11187
---

### Don’t use “the” with format names

When you specify a format name for the `convert` command, do not place `the` in front of it. `the` tells HyperCard to treat the format as a function.

```
seconds -- format name
date -- format name
time -- format name
long date -- format name
the seconds -- returns current time
the date -- returns current date
the time -- returns current time
```

