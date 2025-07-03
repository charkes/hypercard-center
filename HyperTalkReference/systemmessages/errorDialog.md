---
title: errorDialog
card_id: 97279
---

# errorDialog

```
errorDialog [ph:errorMessageText]
```

Handler:

```
on errorDialog [ph:whatText]
  [ph:statements]
end errorDialog
```

HyperCard sends the `errorDialog` message and its text to the current card if it encounters an error when the `lockErrorDialogs` property is set `true`.

(In such a case, the ordinary error dialog box is <u>not</u> displayed.)

`[ph:errorMessageText]` is the contents of the error dialog box that would be displayed if the `lockErrorDialogs` property were `false`.

## Examples

```

on errorDialog what
  if what is "User level is too low to edit scripts."
  then set userLevel to 5
end errorDialog
```

## Demo Script

```
on errorDemo
  set the cantDelete of this card to true
  set lockErrorDialogs to true
  doMenu "Delete Card"
end errorDemo

-- handler in the script of this card
on <b>errorDialog</b> whichError
  answer "Had lockErrorDialogs not been set to true," &&¬
  "HyperCard would have displayed the error, “" & whichError & "”"
end errorDialog
```

## Related Topics

* [lockErrorDialogs](/HyperTalkReference/properties/lockErrorDialogs)
