---
title: Referring to objects
card_id: 11326
modified: yes
---

# Referring to objects

You can refer to HyperCard objects and other elements from a script in any of several ways.

Click Tips for a list of synonyms that you can use for referring to objects.

### name

An object’s name is the value found in its Info dialog box. For example:

`background button "Home"`

It’s a good idea to use quotation marks around an object’s name so that HyperCard recognizes it literally and doesn’t look for a variable by that name.

Note: HyperCard interprets `card "1812"` as a card named `1812`; it interprets `card 1812` as card number `1812`.

### number

An object’s number represents its position among like objects within the object that contains it.

Buttons and fields are ordered within a card or background.  Cards and backgrounds are ordered within a stack.

`go to card 2`

Changing the order of a button, field, card, or background changes its number.

### id

An object or menu's <b>ID</b> is a unique number assigned by HyperCard. Object ID numbers never change. The Info dialog box for each object displays its ID. (Stacks don't have ID's.)

`go to card id 5734`

A program's ID is its application signature:

`put the id of HyperCard -- -> WILD`

### part

<b>Part</b> refers to a specific button or field in its ordinal position among all the buttons and fields in that domain:

```
select part 2
if word 2 of name of part 1 is "button"...
get the name of part 1
set the partNumber of last part to 1
put the number of parts into totalCardParts
put the id of bg part 3 into field idList
```

If you don't specify a domain, the default domain is card.

### ordinal

You can refer to an object using any of the following <b>ordinals</b>:

```
first through tenth
middle, last, any
```

For example:

`go to first card of last background`

### position

You can refer to some objects using any of the following <b>positions</b>:

`next, prev, previous, this`

For example:

```
go to first card of this background
go next card
```

### me

<b>Me</b> is one way to refer to an object dynamically.  It refers to the object that contains the currently executing handler. With buttons and fields, `me` refers to the object itself or to its contents, depending on the context. For example:

```
--In the script of a button:
set the hilite of me to true -- the button
get me -- the contents

--In the script of a field:
select text of me -- selects the field text
select me -- selects the field itself
put empty into me -- replaces the contents
```

### target

The target is another way to refer to an object dynamically. It refers to the object that first received the message currently being handled. With buttons and fields, use `the target` to refer to the field itself and `target` to refer to its contents.

For example:

```
set the hilite of the target to true
select the target --the btn or fld itself
put target --the contents of the btn or fld
put the target --the name of the btn or fld
```
