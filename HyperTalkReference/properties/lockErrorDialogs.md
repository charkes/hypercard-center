---
title: lockErrorDialogs
card_id: 97387
---

# lockErrorDialogs

```
set [the] lockErrorDialogs to [ph:trueOrFalse]
```

The `lockErrorDialogs` property returns or sets whether HyperCard, on encountering an error, presents an error dialog box.

This property defaults to false at idle time, meaning that error dialogs usually appear.

When this property is set to `true`, HyperCard, on encountering an error, does <u>not</u> display an error dialog box; instead, it sends the message `errorDialog [ph:errorMessageText]` to the current card.

`[ph:ErrorMessageText]` contains the text of the error dialog box.

## Examples

```
set lockErrorDialogs to true

set lockErrorDialogs to false
```

## Demo Script

```
on errorDemo
  set the cantDelete of this card to true
  set <b>lockErrorDialogs</b> to true
  doMenu "Delete Card"
end errorDemo

-- handler in the script of this card
on errorDialog whichError
  answer "Had lockErrorDialogs not been set to true," &&¬
  "HyperCard would have displayed the error, “" & whichError & "”"
end errorDialog
```

## Related Topics

* [errorDialog](/HyperTalkReference/systemmessages/errorDialog)
