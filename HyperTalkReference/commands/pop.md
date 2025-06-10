---
title: pop
card_id: 44101
---

# pop

<code><pre>
pop card
pop card { into | after | before }  ¬
       [[ph:chunk] of] [ph:container]
</pre></code>

The <code>pop card</code> command retrieves the identification (full card ID and stack path name) of a card previously saved with the <code>push card</code> command.

If you don’t provide a container to hold the card information, <code>pop</code> goes directly to the popped card.

If you do specify a container, <code>pop</code> puts the card’s identification into the container, and you don’t go anywhere. You can then check the card ID or stack to decide whether you want to return to that card.

## Examples

```
pop card

pop card into theCard
pop card before bkgnd field "History List"
pop card after last line of bkgnd field "History List"
```

## Demo Script

<code><pre>
on goHomeAndBack
 set lockmessages to true -- to leave this field up
 push this card
 go to card 3 of stack "Home"
 wait 30
 <b>pop</b> card
end goHomeAndBack
</pre></code>

## Related Topics

* [go](/HyperTalkReference/commands/go)
* [push](/HyperTalkReference/commands/push)
