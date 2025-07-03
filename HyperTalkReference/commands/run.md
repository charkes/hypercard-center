---
title: run
card_id: 104294
---

# run

```
run
send "run" to [ph:object]
```

The `run` command executes an OSA script.

Used in any other way, `run` does nothing.

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
