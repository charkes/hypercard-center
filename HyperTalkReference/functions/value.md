---
title: value
card_id: 67163
---

# value

<code><pre>
the value of [ph:expression]
</pre></code>

Value returned: the value of the expression after HyperTalk evaluates it


There is no limit to the number of characters that <code>the value </code>can have as its argument. 



When the argument of <code>value</code> is a multitoken literal expression, the expression evaluates to itself:

  <code>put value("HyperCard 2.2")

</code>yields<code> HyperCard 2.2</code> 


## Examples

```
put the value of the clickChunk into theClickedText

the value of "3" & "+2" -- returns 3+2
the value of ("3" & "+2") -- returns 5
```

## Demo Script

<code><pre>
on talkAboutValue
  select last line of me
  answer "The last line of field “Demo Script” is:" & return &&¬
  last line of me & return & return &¬
  "The value of the last line of this field is:" & return &&¬
  the <b>value</b> of last line of me
end talkAboutValue

2 * (3 + 6)/4
</pre></code>

## Related Topics

* [do](/HyperTalkReference/keywords/do)
* [get](/HyperTalkReference/commands/get)
