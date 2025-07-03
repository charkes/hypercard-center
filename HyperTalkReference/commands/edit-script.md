---
title: edit script
card_id: 36226
---

# edit script

<code>edit [the] <code>script of [ph:object]</code>

The <code>edit script</code> command opens the script of an object with the HyperCard script editor.  

When run as a statement in a handler, <code>edit script</code> suspends execution of the handler until the user closes the script editor or activates the card window.

Note: Even though HyperCard itself is an object (it can receive messages), it does <u>not</u> have a script. The following statement yields an error:

```
edit the script of HyperCard
```

For this command to work, the <code>userLevel</code> property must be set to 5.

## Examples

```
edit the script of this card
edit script of background 2
edit script of card button 1 of card 1
edit script of last background part

edit script of stack "Home"
edit script of this stack
```

## Demo Script

```
on openScriptWindow
  set the script of bkgnd field "Demo Script" to¬
  "-- Click the close box to close this script window!"
  <b>edit</b> script of bkgnd field "Demo Script"
end openScriptWindow
```

## Related Topics

* [script](/HyperTalkReference/properties/script)
* [scriptEditor](/HyperTalkReference/properties/scriptEditor)
