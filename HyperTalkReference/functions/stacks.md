---
title: stacks
card_id: 7047
---

# stacks

```
the stacks
```

Value returned: a return-separated list of the full path names for all the open stacks, in front-to-back order

## Examples

```
if the number of lines of the stacks = 1
then ... -- only one stack open
else ... -- multiple stacks open
```

## Demo Script

```
on whatStacks
  put longNamesToShort(<b>the stacks</b>) into theStacks
  answer "The stacks currently open are:" & return & return & theStacks
end whatStacks

function longNamesToShort longStackList
  put empty into shortStackList
  set the itemDelimiter to ":"
  repeat with lineNum = 1 to the number of lines in longStackList
    put last item of line lineNum of longStackList into ¬
    line lineNum of shortStackList
  end repeat
  set itemDelimiter to comma
  return shortStackList
end longNamesToShort
```

## Related Topics

* [windows](/HyperTalkReference/functions/windows)
