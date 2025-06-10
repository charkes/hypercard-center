---
title: help
card_id: 39675
---

# help

<code>help</code>

The <code>help</code> command goes to the first card of the HyperCard Help stack.

HyperCard sends the <code>help</code> command to the current card when the user chooses Help from the Go menu (or presses Command-?).

Note: The command <code>go help</code> is equivalent to <code>go stack "help"</code>, while the <code>help</code> command tries to execute <code>go stack "HyperCard Help"</code>.

You can handle the <code>help</code> message as follows:

<code><pre>
on help
  [ph:statements]
end help
</pre></code>

## Related Topics

* [Commands sent automatically](/HyperTalkReference/systemmessages/Commands-sent-automatically)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
