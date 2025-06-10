---
title: lockErrorDialogs
card_id: 97387
---

# lockErrorDialogs

<code> set </code>[<code>the</code>]<code> lockErrorDialogs to [ph:¬  ]                [ph:trueOrFalse]

</code>The <code>lockErrorDialogs</code> property returns or sets whether HyperCard, on encountering an error, presents an error dialog box.

This property defaults to false at idle time, meaning that error dialogs usually appear. 

 When this property is set to <code>true</code>, HyperCard, on encountering an error, does <u>not</u> display an error dialog box; instead, it sends the message <code>errorDialog [ph:errorMessageText</code> ]to the current card.

[ph:<code>ErrorMessageText </code>]contains the text of the error dialog box. 


## Examples

```

set lockErrorDialogs to true

set lockErrorDialogs to false
```

## Demo Script

<code><pre>
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
</pre></code>

## Related Topics

* [errorDialog](/HyperTalkReference/systemmessages/errorDialog)
