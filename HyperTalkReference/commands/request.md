---
title: request
card_id: 98925
modified: yes
---

# request

```
request [ph:expression] from|of program ¬
   [ph:program]
request [ph:expression] from|of ¬
   program id [ph:programID]
request [ph:expression] from|of ¬
   this program
request appleEvent data|class|id| ¬
   sender|return id|sender id
request appleEvent data ¬
   with keyword [ph:aeKeyword]
```

`[ph:Expression]` yields an expression understandable to the target program.

`[ph:From]` and `[ph:of]` are interchangeable.

`[ph:Program]` yields a valid program path name in the form

`[ph:zone:targetComputer:targetProgram]`

where `[ph:targetProgram]` is the name of a program running on computer `[ph:targetComputer]` in network zone `[ph:zone]`. `[ph:ProgramID]` is the application’s signature. `[ph:AeKeyword]` is an Apple event keyword.

The `request` command sends an “evaluate expression” Apple event from HyperCard to another application.

You can use this command to send an expression to any program that understands the standard `eval` Apple event.

The expression you use must be understandable to the target program. For example, if the target program is another HyperCard, the expression can be any valid HyperTalk expression.

When the target program executes the statement, the result of the request (the value of the expression) goes into the local variable `it`.

If the target program reports an error, HyperCard sets the result with an error message.

You use the `request appleEvent` forms to examine the data and attributes of an incoming Apple event.

You can omit the `[ph:zone]` parameter from the program path name when the target computer is in the same zone as the source computer.

You can omit the `[ph:targetComputer]` parameter if the target program is running on the same computer as HyperCard.

You can pass the user selection from the `answer program` command as the `[ph:program]` parameter.

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

```
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
```

## Placeholders

[embed:HelpExtras/Placeholders/expression.md]

[embed:HelpExtras/Placeholders/Expression.md]

## Related Topics

* [answer](/HyperTalkReference/commands/answer)
* [appleEvent](/HyperTalkReference/systemmessages/appleEvent)
* [reply](/HyperTalkReference/commands/reply)
