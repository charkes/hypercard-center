---
title: The building blocks
card_id: 11056
modified: yes
---

# The building blocks

HyperTalk scripts use a number of basic building blocks as sources of value.

=== basic sources of value

The basic sources of value in HyperTalk are as follows:

* a number ([[c:3]], [[c:-99.9]], and so on)
* a literal, a string of characters set off (delimited) by quotation marks: <code>"The quick brown fox"</code>
* a boolean value ([[c:true]] or [[c:false]])

=== operator

An <b>operator</b> is a character or group of characters that causes a particular calculation or comparison to occur. In HyperTalk, operators operate on values. For example, the plus sign (+) is an arithmetic operator that adds numerical values.

<code><pre>
3 + 4
4 * 5
theCount = 0
the number of card buttons < 10
"this" && "that"
</pre></code>


=== expression

An expression is simply a description of how to get a value; it is either a basic source of value or a complex expression built from sources of value and operators.

For example, the expression <code>8 * (2 + 2)</code> refers to the value `32`.

=== constant

A constant is a named value that never changes. For example:

<code><pre>
empty
pi
return
tab
two
zero
</pre></code>


=== local variable

A local variable is a named container (a place to store values) whose value is whatever you put into it. A local variable is valid only within the handler in which it is used—the variable goes out of existence when the handler ends. You create a local variable by using its name with the put command and putting a value into it. For example, the statement

<code><pre>
put 7 into counter
</pre></code>


puts the value 7 into a variable named counter. (Don’t use quotation marks around the names of variables.)

=== global variable

A global variable is a named container (a place where you can store values) whose value is whatever you choose to put into it, but it is valid for all handlers in which it is declared. To declare a global variable, precede its name with the keyword global:

<code><pre>
on myHandler
   global Total
   put 100 into Total
end myHandler
</pre></code>


You also create a global variable when you put a value into a variable from the Message box.

=== it

<b>It</b> is a pre-defined variable. HyperCard uses it to store information that’s returned by commands such as [[c:ask]], [[c:answer]], [[c:convert]], and [[c:read]]. You can also place a value directly into [[c:it]] using the [[c:get]] command (`put 3 into it` and `get 3` are equivalent). When set in a handler, the value of it is local to the handler. When set from the Message box, the value is global.

Use it when you need a variable temporarily. Use a named, local variable when you want to refer to a value throughout a handler—it’s too easy to change the value of [[c:it]] accidentally.

=== button

A button, like a variable, is also a container (a place where you can store values). The value of a button is equal to whatever text it contains. For example:

<code><pre>
"biscuits" is in bg button "Menu"
</pre></code>


is true if the literal `"biscuits"` appears somewhere in the contents of the button.

As with variables, the text that buttons hold is invisible; as with fields, the text in a button remains there—even between HyperCard sessions—until you change it.

=== field

A field, like a variable, is also a container (a place where you can store values). The value of a field is equal to whatever text it contains. For example:

background field "address" = empty

is true if the field has nothing in it;

"Cupertino" is in card field "Address"

is true if the literal "Cupertino" appears somewhere in the field.  Fields generally contain text you want users to see.

=== message box

The Message box (also called the Message window) is a single-line container.

the Message box is empty

is true if there is nothing in the Message box;

"go" is in the Message box

is true if the literal "go" appears in the
Message box.

=== selection

The selection is a container that holds the currently selected area of text. The text can appear in any field or in the Message box. (Note: text found by the find command is not selected.) The value of the selection equals the text that is highlighted. For example:

the selection is empty
"Cupertino" is in the selection

=== chunk expression

A chunk expression is a description of a unique piece of the contents of any container or other source of value. A chunk expression can refer to a specific character, word (separated by blank spaces), item (separated by commas), line (separated by Return characters), or a combination or range of these. For example:

char 1 of background field "Name"
word 1 to 10 of card field 1
char 1 of word 2 of item 3 of line 4 to 6 ¬ of bkgnd field "Address" of card 20

=== property

A property is a named value that defines a characteristic of a HyperCard object or the HyperCard environment. For example, setting the user level to Scripting changes the userLevel property of HyperCard to the value 5. Properties are often selected as options in dialog boxes or on palettes, and they often can be set from handlers. For example:

get the name of card 1
get the location of the card window
set the name of card 1 to "Index"
set the style of field 1 to "scrolling"

=== function

A function is a named value that HyperCard calculates each time it is used.

The way in which the value is calculated is defined internally for HyperTalk’s built-in functions. You can define your own functions by writing function handlers. Sometimes a script must supply a function with starting values or parameters. By definition, functions return a value. For example:

get the sin of 0
get sin(0)

## Related Topics

* [Writing function handlers](/HyperTalkReference/hypertalkbasics/Writing-function-handlers)
