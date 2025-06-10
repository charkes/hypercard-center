---
title: lockMessages
card_id: 75037
---

# lockMessages

<code> set </code>[<code>the</code>]<code> lockMessages to [ph:trueOrFalse]

</code>The <code>lockMessages</code> property returns or sets whether HyperCard sends certain messages automatically.

The messages affected are<code> closeCard</code>,<code> closeBackground</code>,<code> closeStack</code>,<code> openCard</code>,<code> openBackground</code>,<code> openStack</code>,<code> resumeStack</code>, and<code> suspendStack</code>. 

 Setting <code>lockMessages</code> to true is useful when you want to go to a card to retrieve or save information, but you don’t want to stay there. (The handler will run faster with <code>lockMessages</code> set to true.)

The default setting is false, meaning that HyperCard <u>does</u> send the messages. HyperCard sets <code>lockMessages</code> to false on idle. 


## Examples

```
set the lockMessages to true
```

## Demo Script

<code><pre>
on lockMessagesDemo
  -- The script of this background contains a closeCard handler that
  -- closes this Demo Script field if it is open.
  -- By locking messages, this handler prevents HyperCard from sending
  -- the closeCard message when it goes to the previous card.
  set <b>lockmessages</b> to true
  click at the loc of bkgnd button "Prev"
  click at the loc of bkgnd button "Next"
  set <b>lockmessages</b> to false
end lockMessagesDemo
</pre></code>

## Related Topics

* [go](/HyperTalkReference/commands/go)
* [lock](/HyperTalkReference/commands/lock)
* [lockRecent](/HyperTalkReference/properties/lockRecent)
* [lockScreen](/HyperTalkReference/properties/lockScreen)
* [unlock](/HyperTalkReference/commands/unlock)
