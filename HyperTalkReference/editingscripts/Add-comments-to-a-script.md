---
title: Add comments to a script
card_id: 12290
---

# Add comments to a script

In HyperTalk scripts, two hyphens (`--`) indicate a comment. HyperTalk ignores all commented lines when executing a script.

For example:

```
on mouseUp
  -- Displays a dialog box
  answer "What?" with "No" or "Yes"
  put it -- the user's reply
end mouseUp
```

* To comment several lines at once, drag to select the lines you want to comment, and then choose Comment  from the Script menu (or press Command-–).

* To “uncomment” several lines at  once, drag to select the lines you want to uncomment, and then choose Uncomment from the Script menu (or press Command-=).
