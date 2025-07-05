---
title: Using the dynamic path
card_id: 20813
---

### Using the dynamic path

You can use the dynamic path to your advantage. For example, say that you have a stack with four different backgrounds and that you need to print each one differently. You place a handler called `myPrint` in the stack script:

```
on myPrint
  repeat for the number of bkgnds
    printBkgnd the number of this bg
  end repeat
end myPrint
```


You could place a  handler for `printBkgnd` in the stack script. But since you want the four backgrounds to print different information, you would have to check the number of each background before printing:

```
on printBkgnd bkgndNumber
 if bkgndNumber = 1 then
    [ph:statements]
 else if bkgndNumber = 2 then
    [ph:statements]
 else if bkgndNumber = 3 then
    [ph:statements]
 else
    [ph:statements]
 end if
end printBkgnd
```


But you can use the dynamic path to avoid the `if` statement altogether. To make HyperCard invoke the dynamic path, you should remove the `printBkgnd` handler from the stack script. Then, in the `myPrint` handler, precede the `printBkgnd` statement with the command` go next background`:

```
on myPrint
  repeat for the number of bkgnds
    go next background
    printBkgnd
  end repeat
end myPrint
```


Now `printBkgnd` will travel along the message passing order as usual (the <b>static path</b>) until it reaches HyperCard itself. HyperCard won’t recognize `printBkgnd` as a built-in message, but since the `myPrint` handler has gone to another card, HyperCard invokes the dynamic path. It sends `printBkgnd` again as a message to the current card and passes it through the message passing order from there (the <b>dynamic path</b>).

Now you can place one `printBkgnd` handler in the script of each of the four backgrounds:

```
on printBkgnd
 [ph:statements]
end printBkgnd
```

