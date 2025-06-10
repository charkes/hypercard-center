---
title: Comparison operators
card_id: 89783
modified: yes
---

# Comparison operators

### =, is

Results in<code> true </code>if the expression to its left and the expression to its right have the same values. The expressions can be arithmetic, text, or logical.

<code><pre>
N = 0
word 1 of card field 1 = 10
the name of this card is "Index"
</pre></code>

### <>, ≠,  is not

Results in<code> true </code>if the expression to its left and the expression to its right have different values. The expressions can be arithmetic, text, or logical.

<code><pre>
the number of this card <> 1
the number of this card ≠ 1
the name of this card is not "Index"
</pre></code>

Note: To get the character <code>≠</code>, hold down Option and press <code>=</code>.

### <

Results in <code>true</code> if the expression to its left has a value less than the one to its right. The expressions can be both arithmetic or both text.

<code><pre>
the number of this card < 10
the freesize of this stack < 5120
</pre></code>

### >

Results in<code> true </code>if the expression to its left has a value greater than the one to its right. The expressions can be both arithmetic or both text.

<code><pre>
23 > 13
the version > 1.2.5
(the freesize of this stack) > 10240
</pre></code>

### <=, ≤

Results in <code>true</code> if the expression to its left has a value less than or equal to the one to its right. The expressions can be both arithmetic or both text.

<code><pre>
the number of this card ≤ 10
the freesize of this stack <= 5120
</pre></code>

Note: To get the character <code>≤</code>, hold down Option and press <code><</code>.

### >=, ≥

Results in true if the expression to its left has a value greater than or equal to the one to its right. The expressions can be both arithmetic or both text.

<code><pre>
23 >= 13
the version ≥ 1.2.5
(the freesize of this stack) ≥ 10240
</pre></code>

Note: To get the character <code>≥</code>, hold down Option and press <code>></code>.

### Contains

Results in true if the text string yielded by the expression on its right is found in the text string yielded by the expression on its left (the converse of the operator <code>is in</code>).

<code><pre>
"hello world" contains "lo wo"
the name of this card contains "operator"
</pre></code>

### is in

Results in <code>true</code> if the text string yielded by the expression on its left is found in the text string yielded by the expression on its right (the converse of the operator <code>contains</code>).

<code><pre>
"lo wo" is in "hello world"
"operator" is in the name of this card
</pre></code>

### is not in

Results in <code>true</code> if the text string yielded by the expression on its left is not found in the text string yielded by the expression on its right (the opposite of the operator <code>is in</code>).

<code><pre>
"Apple" is not in "oranges"
"operator" is not in the name of this card
</pre></code>

### is within

Results in <code>true</code> if the point yielded by the expression on its left is contained within the rectangle yielded by the expression on its right.

<code><pre>
"20,20" is within "0,0,40,40"
the mouseLoc is within the rect of ¬
   card button 1
</pre></code>

### is not within

Results in <code>true</code> if the point yielded by the expression on its left is not contained within the rectangle yielded by the expression on its right.

```
"20,20" is not within "0,0,15,15"
the mouseLoc is not within the rect of ¬
   card button 1
```

## Related Topics

* [if (multiple-statement)](/HyperTalkReference/keywords/if-multiple-statement)
* [if (single-statement)](/HyperTalkReference/keywords/if-single-statement)
* [repeat](/HyperTalkReference/keywords/repeat)
* [repeat for](/HyperTalkReference/keywords/repeat-for)
* [repeat until](/HyperTalkReference/keywords/repeat-until)
* [repeat while](/HyperTalkReference/keywords/repeat-while)
* [repeat with](/HyperTalkReference/keywords/repeat-with)
