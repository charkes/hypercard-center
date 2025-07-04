---
title: script
card_id: 80353
---

# script

` set `[`the`]<code> script of [ph:object] to [ph:text]

</code>The `script` property returns or sets a text string equal to the script of the specified object in the current stack or in the stack script of another stack.

When you set the `script` property with the `set` command, you replace the existing script entirely. 


## Examples

```
get the script of card 1
if "mouseUp" is not in it then addMouseUpHandler it

set the script of bkgnd field "Index" to ¬
the script of bkgnd button "Index"

set the script of stack "My Stack" to empty
```

## Demo Script

```
```
on scriptDemo
 answer "The script of this field is:" & ¬
 return & return & the <b>script</b> of me with "OK"
end scriptDemo
```
```

## Related Topics

* [edit script](/HyperTalkReference/commands/edit-script)
* [scriptEditor](/HyperTalkReference/properties/scriptEditor)
* [scriptTextFont](/HyperTalkReference/properties/scriptTextFont)
* [scriptTextSize](/HyperTalkReference/properties/scriptTextSize)
* [Set the font and size of a script](/HyperTalkReference/editingscripts/Set-the-font-and-size-of-a-script)
