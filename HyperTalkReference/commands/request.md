---
title: request
card_id: 98925
modified: yes
---

# request

<code><pre>
request <i>expression</i> from|of program ¬
   <i>program</i>
request <i>expression</i> from|of ¬
   program id <i>programID</i>
request <i>expression</i> from|of ¬
   this program
request appleEvent data|class|id| ¬
   sender|return id|sender id
request appleEvent data ¬
   with keyword <i>aeKeyword</i>
</pre></code>


`<i>Expression</i>` yields an expression understandable to the target program.

<i><code>From</i> </code>and <i><code>of</i> </code>are interchangeable.

<i><code>Program</i> </code>yields a valid program path name in the form

<i><code>zone:targetComputer:targetProgram </i> </code>where <i><code>targetProgram</i> </code>is the name of a program running on computer<code> <i>targetComputer</i> </code>in network zone <i><code>zone</code> </i>.<code> <i>ProgramID</i> </code>is the application’s signature.<code> <i>AeKeyword</i> </code>is an Apple event keyword.

The<code> request </code>command sends an “evaluate expression” Apple event from HyperCard to another application.

You can use this command to send an expression to any program that understands the standard<code> eval </code>Apple event.

The expression you use must be understandable to the target program. For example, if the target program is another HyperCard, the expression can be any valid HyperTalk expression.

When the target program executes the statement, the result of the request (the value of the expression) goes into the local variable<code> it</code>.

If the target program reports an error, HyperCard sets the result with an error message.

You use the<code> request appleEvent </code>forms to examine the data and attributes of an incoming Apple event.

You can omit the <i><code>zone</i> </code>parameter from the program path name when the target computer is in the same zone as the source computer.

You can omit the<i> <code>targetComputer </i></code>parameter if the target program is running on the same computer as HyperCard.

You can pass the user selection from the<code> answer program</code> command as the <i><code>program</i></code> parameter.

## Examples

```
request "the number of cards" from program "KZone:PMac:HyperCard"
request "the name of this stack" of program "HyperCard"
request "{target}" from program "MPW Shell"

The following handler shows how the request command can get information from another HyperCard program:

on getStackName -- handler in source stack
  global HildaPath -- path to another HyperCard
  request "the long name of this stack" ¬
  from program HildaPath
  if the result is empty then answer "Now browsing stack:" && it
  else answer "An error occurred:" && the result
end getStackName
```

## Demo Script

<code><pre>
on tellTheStack
  -- this demo only works with System 7
  if not systemSeven() then exit tellTheStack
  <b>request</b> "the name of this stack" of program ¬
  (the short name of HyperCard)
  answer "This is" && it & "."
end tellTheStack

function systemSeven
  return the systemVersion ≥ 7.0
end systemSeven
</pre></code>

## Placeholders

[embed:HelpExtras/Placeholders/expression.md]

[embed:HelpExtras/Placeholders/Expression.md]

## Related Topics

* [answer](/HyperTalkReference/commands/answer)
* [appleEvent](/HyperTalkReference/systemmessages/appleEvent)
* [reply](/HyperTalkReference/commands/reply)
