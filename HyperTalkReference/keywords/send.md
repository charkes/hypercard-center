---
title: send
card_id: 29297
modified: yes
---

# send

<code><pre>
send "<i>messageName</i> [<i>parameterList</i>]"¬
   [to <i>object</i>]

send "<i>messageName</i> [<i>parameterList</i>]"¬
   to HyperCard

send <i>expression</i>  to { program ¬
   <i>program</i> | program id <i>programID</i> | ¬
    this program } [without reply]
</pre></code>


In the first two forms, the<code> send </code>keyword sends a message directly to a particular object or to HyperCard. For example, you can send a message to an object already passed by  in the message-  passing order (from a stack back to the current card), or you can bypass handlers later in the message-passing order that might otherwise handle the message.

You can send messages to any object in the current stack, and you can send messages to another stack (but not to objects within another stack).

<b>Important</b>: If you send a message to a card other than the current card, HyperCard doesn’t go to the card or open it.

For example, if you send a message to another stack, and the handler refers to a field that’s specific to that stack, you’ll get a script error.

HyperCard evaluates any parameters before it sends the message, even though the entire message is in quota- tion marks. (You don’t need quotation marks if the message is a single word.)

When an object receives a message from send, HyperCard sets the value of the target to the name of the object.

If the object doesn’t handle the message, the message continues along the message-passing path from that point.

If you send a message directly to HyperCard, you ensure that no other objects will handle the message. For example, `send "doMenu next" to HyperCard` always takes you to the next card.

You can type send as a message in the Message box.

The third form sends a do script Apple event from HyperCard to another running application:

<code><pre>
send expression  to { program ¬
   <i>program</i> | program id <i>programID</i> | ¬
   this program }  [without reply]
</pre></code>


where program is the path name to the target program in the form <i>zone:computer:program</i>, and <i>programID</i> is the signature of a program on the same computer. this program denotes HyperCard.

<i>expression</i> is any valid expression or any sequence of commands in the scripting language supported by the target program. If the target program is HyperCard, the scripting language is HyperTalk.

By default, HyperCard waits for a reply from the target program before continuing; but you can specify  `without reply`  if  you don't want to wait for one.

Any reply from the target program goes into `the result`.

## Examples

```
send "hideIt" to field 3  
send "addSums 3,45.67,344.00" to stack "Expense Account"  
send "mouseUp" to button "Click Me"  
send "doMenu" && quote & "print card" & quote to HyperCard
```

## Demo Script

<code><pre>
on sendDemo
  <b>send</b> "mouseDown" to bkgnd btn "close" -- to animate the close box
  wait 20
  <b>send</b> "mouseUp" to bkgnd btn "close" -- to put away this demo
end sendDemo
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/messageName.md]

[embed:HelpExtras/Placeholders/parameterList.md]

[embed:HelpExtras/Placeholders/object.md]

[embed:HelpExtras/Placeholders/expression.md]

## Related Topics

* [on](/HyperTalkReference/keywords/on)
* [pass](/HyperTalkReference/keywords/pass)
* [run](/HyperTalkReference/commands/run)
* [target](/HyperTalkReference/functions/target)
* [The message-passing order](/HyperTalkReference/hypertalkbasics/The-message-passing-order)
