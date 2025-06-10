---
title: controlKey
card_id: 33000
---

# controlKey

<code>controlKey [ph:posInteger]</code>

The <code>controlKey</code> command has no built-in effect. HyperCard sends the <code>controlKey</code> command to the current card when a combination of the Control key and another key is pressed.

You can handle the <code>controlKey</code> message as follows:

<code><pre>
on controlKey theKeyNumber
  [ph:statements]
end controlKey
</pre></code>

HyperCard passes the following numbers for each control key combination:

[TODO:Format table here]

## Examples

```
 -- same as holding down Control + left arrow; no built in effect:
controlKey 28

on controlKey whichKey
  if whichKey is 28 then go previous marked card
  else if whichKey is 29 then go next marked card
  else pass controlKey
end controlKey
```

## Related Topics

* [Commands sent automatically](/HyperTalkReference/systemmessages/Commands-sent-automatically)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
