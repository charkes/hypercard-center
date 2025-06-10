---
title: run
card_id: 104294
---

# run

<code><pre>
run
send "run" to [ph:object]
</pre></code>

The <code>run</code> command executes an OSA script.

Used in any other way, <code>run</code> does nothing.

## Examples

```
send "run" to button "Automatic"  -- invoke attached QuicKeys script

send "run" to button "Quill"  -- invoke implicit AppleScript run handler

on mouseUp
  run  -- invoke AppleScript in card script
end mouseUp
```

## Related Topics

* [send](/HyperTalkReference/keywords/send)
