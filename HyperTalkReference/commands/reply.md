---
title: reply
card_id: 97817
modified: yes
---

# reply

```
reply [ph:expression] [with keyword ¬
   [ph:aeKeyword]]
reply error [ph:expression]
```

`[ph:Expression]` is any text. `[ph:AeKeyword]` is an Apple event keyword (a 4-character string).

The `reply` command answers an incoming Apple event.

If you don’t specify a keyword, `[ph:expression]` becomes the direct parameter of the reply.

You use `reply error [ph: expression]` to notify the Apple event sender that an error has occurred.

You can use `reply error [ph: expression]` to define your own error messages. This form is equivalent to `reply [ph:expression] with keyword "errs"`.  The Apple event keyword “`errn`” sets the error number.

The reply command sets the result to `No current Apple event` when there is no current Apple event to handle.

Use `reply` only if you're handling Apple events yourself. If HyperCard handles an Apple event, it will provide the appropriate information in the reply.

See the documentation for the sending program to know which `reply` keywords it expects. (`errs` and `errn` are standard keywords.)

In AppleScript, you may need to reply with both an error string and an error number to trigger an error clause.

## Examples

```
reply "Hello there, nice to hear from you"
reply error "Error in the remote stack"
reply 13023 with keyword "errn"  -- Error #13023 occurred

The following script handles Apple events of class WILD and type defn. It searches for a string in a background field name ”Glossary Entry” and ret  urns the contents of a background field named “Definition.”

on appleEvent eventClass, eventID, sender
  if eventClass is "WILD" and eventID is "defn" then
    request appleEvent data
    find it in field "Glossary Entry"
    if the result is empty     -- find is successful
    then reply field "Definition"
    else reply error "Not found"
  else pass appleEvent
end appleEvent
```

## Related Topics

* [appleEvent](/HyperTalkReference/systemmessages/appleEvent)
* [request](/HyperTalkReference/commands/request)
