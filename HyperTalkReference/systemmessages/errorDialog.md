---
title: errorDialog
card_id: 97279
---

# errorDialog

<code><pre>
errorDialog [ph:errorMessageText]
</pre></code>

Handler:

<code><pre>
on errorDialog [ph:whatText]
  [ph:statements]
end errorDialog
</pre></code>

HyperCard sends the <code>errorDialog</code> message and its text to the current card if it encounters an error when the <code>lockErrorDialogs</code> property is set<code> true</code>.

(In such a case, the ordinary error dialog box is <u>not</u> displayed.) 

 [ph:<code>errorMessageText </code>]is the contents of the error dialog box that would be displayed if the <code>lockErrorDialogs</code> property were <code>false</code>. 


## Examples

```

on errorDialog what
  if what is "User level is too low to edit scripts." 
  then set userLevel to 5
end errorDialog
```

## Demo Script

<code><pre>
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
</pre></code>

## Related Topics

* [lockErrorDialogs](/HyperTalkReference/properties/lockErrorDialogs)
