---
title: functionKey
card_id: 38567
---

# functionKey

<code>functionKey [ph:posInteger</code>]

Note: <code> [ph:posInteger] </code>must yield a number between 1 and 15.

HyperCard sends the <code>functionKey</code> command to the current card when the user presses one of the function keys on the Apple Extended Keyboard.

The <code>functionKey</code> command performs an undo, cut, copy, or paste for the values 1 through 4. Integer values 5 through 15 have no built-in effect. 

You can handle the <code>functionKey</code> message as follows:

<code><pre>
on functionKey whichKey
  [ph:statements]
end functionKey
</pre></code>


## Examples

```
functionKey 1 -- performs undo
functionKey 2 -- performs cut
functionKey 3 -- performs copy
functionKey 4 -- performs paste

  
-- An example handler:

on functionKey whichKey  
  if whichKey is 5 then myCoolHandler
  else if whichKey is 6 then choose browse tool 
  else if whichKey is 7 then choose button tool
  else if whichKey is 8 then choose field tool
  else pass functionKey
end functionKey
```

## Related Topics

* [Commands sent automatically](/HyperTalkReference/systemmessages/Commands-sent-automatically)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
