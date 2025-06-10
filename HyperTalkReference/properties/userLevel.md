---
title: userLevel
card_id: 87536
---

# userLevel

<code> set </code>[<code>the</code>]<code> userLevel to [ph:posInteger]

</code>where <code>[ph:posInteger]</code> is 1, 2, 3, 4, or 5.

The <code>userLevel</code> property returns or sets the user level as follows:

<code><pre>
1  = Browsing
2  = Typing
3  = Painting
4  = Authoring
5  = Scripting
</pre></code>



 HyperCard determines the default setting for <code>userLevel</code> from the Preferences card of the Home stack at startup and when HyperCard resumes after being suspended. 


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

<code><pre>
on whatUserLevel
  answer "The current user level is:" && the userLevel
end whatUserLevel
</pre></code>

## Related Topics

* [blindTyping](/HyperTalkReference/properties/blindTyping)
* [powerKeys](/HyperTalkReference/properties/powerKeys)
* [textArrows](/HyperTalkReference/properties/textArrows)
