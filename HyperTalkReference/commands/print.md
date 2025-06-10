---
title: print
card_id: 44420
modified: yes
---

# print

<code><pre>
print card [from <i>point1</i> to <i>point2</i>]
print all cards
print marked cards
print <i>posInteger</i> cards
print <i>card</i> [from <i>point1</i> to <i>point2</i>]
print {<i>field</i> | <i>button</i> }
print <i>fileName</i> with <i>application</i>
print <i>expression</i>
</pre></code>


The<code> print </code>command prints card images, the contents of fields and buttons, documents from other programs, or the value of any HyperTalk expression.

<code>Print card </code>prints an image of the current card. The option<code> from <i>point1</i> to <i>point2</i> </code>specifies a rectangular area of the card.

<code>Print all cards </code>prints the image of every card in the stack.

<code>Print marked cards </code>prints a subset of the cards in the stack based on each card’s<code> marked </code>property (as reflected in its Card Info dialog box). You can mark cards with the<code> mark </code>command.

<code>Print <i>posInteger</i> cards </code>prints a range of consecutive cards starting from the current card.

<code>Print <i>card</i> </code>prints the card specified by the card expression. The option<code> from <i>point1</i> to <i>point2</i> </code>specifies a rectangular area of the card. HyperCard sets the function<code> the result </code>to<code> "No such card." </code>if the specified card doesn’t exist; otherwise,<code> the result </code>returns<code> empty</code>.

<code>Print</code> <i><code>button</i> </code>prints the contents of the specified button.

<code>Print</code> <i><code>field</i> </code>prints the contents of the specified field, preserving the fonts, sizes, and styles of text used in the field.

<code>Print file with application </code>prints a document using another program. HyperCard launches the application; the application tries to print the document. (The user might see a Print dialog box.)

If HyperCard can't find either the document or the application, it displays a directory dialog box and asks the user to find it.

HyperCard also sets<code> the result </code>to<code> Cancel </code>if the user clicks Cancel in the dialog box. Otherwise, it sets<code> the result </code>to<code> empty</code>.

If HyperCard has problems opening the application (for example, there’s not enough memory), it sets<code> the result </code>to<code> "Couldn't open that application."</code>

After printing, the application program quits, and control returns to HyperCard.

Finally,<code> print <i>expression</i> </code>prints the value of any HyperTalk expression. You can print the values of local and global variables, fields, <i><code>chunk</i> </code>expressions, the current selection, the contents of the Message box, and the result of any function or property.

Expressions are printed using the settings in<code> printMargins, printTextAlign, printTextFont, printTextSize, printTextHeight, </code>and<code> printTextStyle</code>.

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

<code><pre>
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
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/posInteger.md]

[embed:HelpExtras/Placeholders/card.md]

[embed:HelpExtras/Placeholders/field.md]

[embed:HelpExtras/Placeholders/button.md]

[embed:HelpExtras/Placeholders/fileName.md]

[embed:HelpExtras/Placeholders/application.md]

[embed:HelpExtras/Placeholders/expression.md]

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
