---
title: type
card_id: 49918
---

# type

<code><pre>
type [ph:text]
type [ph:text] with commandKey
</pre></code>

The <code>type</code> command <code></code>acts exactly as if the user had typed<code> [ph:text]</code> from the keyboard.

The text appears in the Message box when it’s visible (or also when it’s hidden if <code>blindTyping</code> is set to <code>true</code>).

To type text into a field or to add paint text, a handler must first set the insertion point (using either the <code>select</code> or <code>click at</code> command).

To perform a menu command, use the form<code> type [ph:text] with commandKey</code>. For example, if you have a graphic on the Clipboard, you can paste it with the command

<code>type "V" with commandKey</code>

## Examples

```
type "Hello there world" -- in the Message box

select before text of card field 1
type "Hello there world"

type "P" with commandKey -- print card  
type "V" with commandKey,shiftKey -- paste a field and its text
```

## Demo Script

<code><pre>
on typeIntoMe
  show bkgnd field "demo field"
  set the lockText of bkgnd field "demo field" to false
  select text of bkgnd field "demo field"
  type line 6 of bkgnd field "Help Text A"
  type return & return & "Click the mouse to continue..."
  select empty
  wait until the mouseClick
  hide bkgnd field "demo field"
  set the lockText of bkgnd field "demo field" to true
end typeIntoMe
</pre></code>

## Related Topics

* [click at](/HyperTalkReference/commands/click-at)
