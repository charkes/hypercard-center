---
title: print
card_id: 44420
modified: yes
---

# print

```
print card [from [ph:point1] to [ph:point2]]
print all cards
print marked cards
print [ph:posInteger] cards
print [ph:card] [from [ph:point1] to [ph:point2]]
print {[ph:field] | [ph:button] }
print [ph:fileName] with [ph:application]
print [ph:expression]
```

The `print` command prints card images, the contents of fields and buttons, documents from other programs, or the value of any HyperTalk expression.

`Print card` prints an image of the current card. The option `from [ph:point1] to [ph:point2]` specifies a rectangular area of the card.

`Print all cards` prints the image of every card in the stack.

`Print marked cards` prints a subset of the cards in the stack based on each card’s `marked` property (as reflected in its Card Info dialog box). You can mark cards with the `mark` command.

`Print [ph:posInteger] cards` prints a range of consecutive cards starting from the current card.

`Print [ph:card]` prints the card specified by the card expression. The option `from [ph:point1] to [ph:point2]` specifies a rectangular area of the card. HyperCard sets the function `the result` to `"No such card."` if the specified card doesn’t exist; otherwise, `the result` returns `empty`.

`Print [ph:button]` prints the contents of the specified button.

`Print [ph:field]` prints the contents of the specified field, preserving the fonts, sizes, and styles of text used in the field.

`Print file with application` prints a document using another program. HyperCard launches the application; the application tries to print the document. (The user might see a Print dialog box.)

If HyperCard can't find either the document or the application, it displays a directory dialog box and asks the user to find it.

HyperCard also sets `the result` to `Cancel`if the user clicks Cancel in the dialog box. Otherwise, it sets `the result` to `empty`.

If HyperCard has problems opening the application (for example, there’s not enough memory), it sets `the result` to `"Couldn't open that application."`

After printing, the application program quits, and control returns to HyperCard.

Finally,`print [ph:expression]` prints the value of any HyperTalk expression. You can print the values of local and global variables, fields, `[ph:chunk]` expressions, the current selection, the contents of the Message box, and the result of any function or property.

Expressions are printed using the settings in `printMargins, printTextAlign, printTextFont, printTextSize, printTextHeight,` and `printTextStyle`.

## Examples

```
print card
print card from 0,0 to 100,100
print card from topLeft of this card to the clickLoc

print first card
print this card
print card id 19390 from 90,0 to 180,180

-- Print marked cards:
print marked cards -- all of them
print next marked card
print second marked card
print marked card 5

print 10 cards
print (the number of cards of this bg) cards

-- Print a document using another program:
print "Read Me" with "Teach Text"
if the result is not empty then ... -- didn't print it

-- Print a field (preserves text styles):
print background field 1


-- Print any expression (no text styles):
print card field 1 & return & card field 2
print the selection
print the Message box
print "Hello there world"
print myVariable
```

## Demo Script

```
on printDemo
  answer "Are you connected to a printer?" with "No" or "Yes"
  if it is "No" then exit printDemo
  lock screen
  open printing
  repeat with cardOffSet = 0 to 2
    <b>print card</b> (the number of this card + cardOffSet)
  end repeat
  close printing
  unlock screen
end printDemo
```

## Related Topics

* [close](/HyperTalkReference/commands/close)
* [mark](/HyperTalkReference/commands/mark)
* [open printing](/HyperTalkReference/commands/open-printing)
* [open report printing](/HyperTalkReference/commands/open-report-printing)
* [printMargins](/HyperTalkReference/properties/printMargins)
* [printTextAlign](/HyperTalkReference/properties/printTextAlign)
* [printTextFont](/HyperTalkReference/properties/printTextFont)
* [printTextHeight](/HyperTalkReference/properties/printTextHeight)
* [printTextSize](/HyperTalkReference/properties/printTextSize)
* [printTextStyle](/HyperTalkReference/properties/printTextStyle)
* [reset](/HyperTalkReference/commands/reset)
