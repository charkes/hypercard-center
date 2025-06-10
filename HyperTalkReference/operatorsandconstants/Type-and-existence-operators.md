---
title: Type and existence operators
card_id: 6157
modified: yes
---

# Type and existence operators

### is a, is an

Results in <code>true</code> if the expression to its left is the same type as the type identifier on the right. The type identifiers are: <code>number</code>, <code>integer</code>, <code>point</code>, <code>rect</code>, <code>date</code>, and <code>logical</code>.

<code><pre>
23 is a number      -- true
pi is an integer    -- false
"0,0,0" is a point  -- false
"0,0,0,0" is a rect -- true
"8/09/65" is a date -- true
false is a logical  -- true
</pre></code>

### there is a, there is an

Results in <code>true</code> if the expression to the right of the operator exists. The expression can take any of the following forms (with appropriate adjectives and/or names):

<code><pre>
window    menu     menuItem   stack
file      disk     document   application
folder    picture  field      program [ID]*
button    part     scriptingLanguage
card      background
*Under system 7 only
</pre></code>

### there is no

Results in <code>true</code> if the expression to the right of the operator does not exist. The expression can identify the same elements as <code>there is a</code>.

<code><pre>
there is no window "message watcher"
there is no menu "MayBe"
there is no menuItem "Back" of menu "Go"
there is no file "Simonides:References"
there is no stack "Home"
there is no card button 1
there is no disk "External Hard Disk"
there is no card 6
there is no bkgnd "fish bowl sizes"
</pre></code>

### there is not a

Same as the operator <code>there is no</code>.

## Related Topics

* [if (multiple-statement)](/HyperTalkReference/keywords/if-multiple-statement)
* [if (single-statement)](/HyperTalkReference/keywords/if-single-statement)
* [repeat](/HyperTalkReference/keywords/repeat)
* [repeat for](/HyperTalkReference/keywords/repeat-for)
* [repeat until](/HyperTalkReference/keywords/repeat-until)
* [repeat while](/HyperTalkReference/keywords/repeat-while)
* [repeat with](/HyperTalkReference/keywords/repeat-with)
