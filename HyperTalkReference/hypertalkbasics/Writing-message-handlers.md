---
title: Writing message handlers
card_id: 9950
modified: yes
---

# Writing message handlers

When you write a handler for a message, you specify a sequence of statements for HyperCard to run. Each message handler has the following form, with the italicized words as placeholders:

<code><pre>
on <i>messageName</i>
    <i>statements</i>
end <i>messageName</i>
</pre></code>


When it runs the message handler, HyperCard sends each line of the handler as a message itself (so handlers can call other handlers).

<b>Important</b>: The message name does <i>not</i> have to be one of HyperCard’s built-in system messages or commands.

For example, if you wanted a new command called<code> doubleBeep </code>that would beep twice, you would write a handler for it as follows:

<code><pre>
on doubleBeep
   beep
   beep
end doubleBeep
</pre></code>


Of course, HyperCard doesn’t know about the [[c:doubleBeep]] command, so it will never be sent automatically in response to an event. But you can send [[c:doubleBeep]] from the Message box or use it as a statement in other handlers.

For example, the script of a card button might contain the following handler for the system message [[c:mouseUp]]:

<code><pre>
on mouseUp
  doubleBeep
end mouseUp
</pre></code>


If the script also contains the [[c:doubleBeep]] handler (or if the script of any object later in the message-passing path contains it), the [[c:mouseUp]] message will send the [[c:doubleBeep]] message, and [[c:doubleBeep]] will send two [[c:beep]] commands. Because [[c:beep]] is a built-in command, HyperCard beeps twice.

If HyperCard can’t find the [[c:doubleBeep]] message, it will complain (with a dialog box) that it “can’t understand” the message.

## Placeholders

[embed:HelpExtras/Placeholders/messageName.md]

[embed:HelpExtras/Placeholders/statements.md]

## Related Topics

* [Handling messages](/HyperTalkReference/hypertalkbasics/Handling-messages)
* [on](/HyperTalkReference/keywords/on)
* [The message-passing order](/HyperTalkReference/hypertalkbasics/The-message-passing-order)
* [Using parameter variables](/HyperTalkReference/hypertalkbasics/Using-parameter-variables)
* [What are messages?](/HyperTalkReference/hypertalkbasics/What-are-messages)
