---
title: menus
card_id: 58014
---

# menus

<code><pre>
the menus
</pre></code>

Value returned: a return-separated list of the names of the menus in the current menu bar

If HyperCard is running under System 7, the list includes the System 7 menus (such as System Help and Application).

Note: The string <code>Apple</code> is a synonym for the  menu. 


## Examples

```
get the menus
if "Objects" is not in it then ...

get menus()
if "Paint" is not in it then ...
```

## Related Topics

* [checkMark](/HyperTalkReference/properties/checkMark)
* [commandChar](/HyperTalkReference/properties/commandChar)
* [create](/HyperTalkReference/commands/create)
* [disable](/HyperTalkReference/commands/disable)
* [doMenu](/HyperTalkReference/commands/doMenu)
* [enable](/HyperTalkReference/commands/enable)
* [enabled](/HyperTalkReference/properties/enabled)
* [markChar](/HyperTalkReference/properties/markChar)
* [menuMessage](/HyperTalkReference/properties/menuMessage)
* [put](/HyperTalkReference/commands/put)
* [reset](/HyperTalkReference/commands/reset)
