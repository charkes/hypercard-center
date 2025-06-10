---
title: enabled
card_id: 71193
---

# enabled

<code><pre>
set [the] enabled of{[ph:menu]|[ph:menuItem ]}¬
   to [ph:trueOrFalse]
</pre></code>

<code>set</code> [<code>the</code>] <code>enabled of [ph:button] ¬     to [ph:trueOrFalse]

</code>The <code>enabled</code> property returns or sets whether a menu item, menu, or button is active or inactive (dimmed). Users cannot choose dimmed elements.   

If you set the <code>enabled</code> of a menu to false, <u>all</u> items on the menu become inactive. 

The <code>enabled</code> property won't enable items in HyperCard’s menus unless they're currently available to the user. 

For example, the following code won't enable the Button Info command unless a button is selected:

<code><pre>
set the enabled of menuItem 1 of ¬ menu "Objects" to true
</pre></code>

The default state is<code> true</code>, meaning that the element is enabled. 


## Examples

```
set the enabled of menu "File" to true
set the enabled of menu 2 to false
set the enabled of second menu to true

set the enabled of menuItem "New" of menu "File" to false
set the enabled of menuItem 2 of menu 2 to true
set the enabled of second menuItem of second menu to false

set the enabled of button 5 to false
if the enabled of bg btn "Scores" is true then show field "Players"
```

## Demo Script

<code><pre>
on mouseUp
  if there is a menu "Reference"
  then set <b>enabled</b> of menuItem 4 of menu "Reference" to ¬
       not (enabled of menuItem 4 of menu "Reference")
end mouseUp
</pre></code>

## Related Topics

* [checkMark](/HyperTalkReference/properties/checkMark)
* [commandChar](/HyperTalkReference/properties/commandChar)
* [create](/HyperTalkReference/commands/create)
* [disable](/HyperTalkReference/commands/disable)
* [doMenu](/HyperTalkReference/commands/doMenu)
* [enable](/HyperTalkReference/commands/enable)
* [markChar](/HyperTalkReference/properties/markChar)
* [menus](/HyperTalkReference/functions/menus)
* [menuMessage](/HyperTalkReference/properties/menuMessage)
* [put](/HyperTalkReference/commands/put)
* [reset](/HyperTalkReference/commands/reset)
