---
title: Properties of the Variable Watcher
card_id: 5882
---

### Properties of the Variable Watcher

Use the following two properties to change the position of the horizontal and vertical bars that divide the Variable Watcher window:

```
set [the] hBarLoc of window ¬
    "Variable Watcher" to [ph:posInteger]
```

sets the position of the horizontal bar to `[ph:posInteger]` pixels from the top of the window. The horizontal bar determines how many of the variable name and value fields appear in the window.

```
set [the] vBarLoc of window ¬
    "Variable Watcher" to [ph:posInteger]
```

sets the position of the vertical bar to `[ph:posInteger]` pixels from the left of the window. The vertical bar separates the variable names from their values.
