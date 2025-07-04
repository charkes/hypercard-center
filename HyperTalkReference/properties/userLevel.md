---
title: userLevel
card_id: 87536
---

# userLevel

` set `[`the`]<code> userLevel to [ph:posInteger]

</code>where `[ph:posInteger]` is 1, 2, 3, 4, or 5.

The `userLevel` property returns or sets the user level as follows:

```
1  = Browsing
2  = Typing
3  = Painting
4  = Authoring
5  = Scripting
```



 HyperCard determines the default setting for `userLevel` from the Preferences card of the Home stack at startup and when HyperCard resumes after being suspended. 


## Examples

```
set the userLevel to 5

if the userLevel < 4 then ...

-- Save and restore the user level:
put the userLevel into savedUserLevel
set the userLevel to 5
... -- do stuff here
set the userLevel to savedUserLevel
```

## Demo Script

```
on whatUserLevel
  answer "The current user level is:" && the userLevel
end whatUserLevel
```

## Related Topics

* [blindTyping](/HyperTalkReference/properties/blindTyping)
* [powerKeys](/HyperTalkReference/properties/powerKeys)
* [textArrows](/HyperTalkReference/properties/textArrows)
