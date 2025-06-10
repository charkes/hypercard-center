---
title: foundLine
card_id: 56528
---

# foundLine

<code><pre>
the foundLine
</pre></code>

Value returned: a line expression equal to the line of a field where the most recent <code>find</code> command located its target string. If nothing was found, it returns<code> empty</code>.  

The line expression has the following form:

<code><pre>
line [ph:i] of card field [ph:n]
line [ph:i] of bkgnd field <i>n
</pre></code>

</i> 

where <code>[ph:i]</code> is the line number and<code> [ph:n] </code>is the number of the field.

Note: A return character determines a line, not the line wrap. A line that wraps and is displayed as two lines is treated as one line by HyperTalk. 


## Examples

```
find "Ann"
put the foundLine

-- Using foundLine to select a line:
find currentTopic in field "Topics"
select word 1 to 2 of the foundLine
```

## Demo Script

<code><pre>
on foundLineDemo
  set cursor to watch
  find string "on foundLineDemo"
  answer "The foundLine is" && the <b>foundLine</b> & "." & return ¬
  & return & "The value of the foundLine is “" &¬
  the value of the <b>foundLine</b> & "”."
end foundLineDemo
</pre></code>

## Related Topics

* [clickLine](/HyperTalkReference/functions/clickLine)
* [find](/HyperTalkReference/commands/find)
* [selectedLine](/HyperTalkReference/functions/selectedLine)
