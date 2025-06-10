---
title: on
card_id: 26982
modified: yes
---

# on

<code><pre>
on <i>messageName</i> [<i>parameterList</i>]
    <i>statements</i>
end <i>messageName</i>
</pre></code>

<br>
The<code> on </code>keyword defines a new message handler of the specified name.<br>
<br>
The optional<code> <i>parameterList</i> </code>lets the handler receive values sent along with a message. HyperCard assigns each value to a parameter variable in the<code> <i>parameterList</i></code>.<br>

## Demo Script

<code><pre>
<b>on</b> mouseUp
  flashTheButton "bkgnd btn id 57",2
<b>end</b> mouseUp

<b>on</b> flashTheButton whichBtn, howMany
  repeat for (howMany * 2) times
    set the hilite of whichBtn to not the hilite of whichBtn
  end repeat
<b>end</b> flashTheButton
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/messageName.md]

[embed:HelpExtras/Placeholders/parameterList.md]

[embed:HelpExtras/Placeholders/statements.md]

## Related Topics

* [exit](/HyperTalkReference/keywords/exit)
* [Handling messages](/HyperTalkReference/hypertalkbasics/Handling-messages)
* [param](/HyperTalkReference/functions/param)
* [paramCount](/HyperTalkReference/functions/paramCount)
* [params](/HyperTalkReference/functions/params)
* [pass](/HyperTalkReference/keywords/pass)
* [result](/HyperTalkReference/functions/result)
* [return](/HyperTalkReference/keywords/return)
* [send](/HyperTalkReference/keywords/send)
* [target](/HyperTalkReference/functions/target)
* [The message-passing order](/HyperTalkReference/hypertalkbasics/The-message-passing-order)
* [Using parameter variables](/HyperTalkReference/hypertalkbasics/Using-parameter-variables)
* [What are messages?](/HyperTalkReference/hypertalkbasics/What-are-messages)
* [Writing message handlers](/HyperTalkReference/hypertalkbasics/Writing-message-handlers)
