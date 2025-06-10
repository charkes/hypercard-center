---
title: foundText
card_id: 56722
---

# foundText

<code><pre>
the foundText
</pre></code>

Value returned: a string equal to the characters enclosed in the box after the most recent <code>find</code> command has located its target string. If nothing was found, it returns<code> empty</code>. 


## Examples

```
find "Jo"
put the foundText

--Using foundText for  conditional processing:
find "Edd" in field "last names"
if the foundText is "Eddings" then
   multiply hoursWorked by 35.50
else
   multiply hoursWorked by 25.50
end if
```

## Demo Script

<code><pre>
<code><pre>
on foundTextDemo
 set cursor to watch
 find string "TextDemo" in field "Demo Script"
 answer "The foundText is “" & the <b>foundText</b> & "”."
end foundTextDemo
</pre></code>
</pre></code>

## Related Topics

* [clickText](/HyperTalkReference/functions/clickText)
* [find](/HyperTalkReference/commands/find)
* [selectedText](/HyperTalkReference/functions/selectedText)
