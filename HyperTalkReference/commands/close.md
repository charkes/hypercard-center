---
title: close
card_id: 32483
modified: yes
---

# close

<code><pre>
close printing
close file <i>fileName</i>
close [<i>document</i> { in | with } ] ¬
            <i>application</i>
close { <i>externalWindow</i> | card window}
</pre></code>


The<code> close printing </code>command ends a print job previously begun with an<code> open printing </code>command.

The<code> close file </code>command closes a disk file previously opened with the<code> open file </code>command. Usually, you open files to import or export text. Always use<code> close file </code>when you’re finished.

If you try to close an unopened file,<code> the result </code>gets<code> File not open.</code>

HyperCard automatically closes all open files when

* it runs an<code> exit to HyperCard </code>    statement,
* the user presses Command-. (Command-period), or
* the user quits HyperCard.

You must provide the full path name of the file if it’s not at the same directory level as HyperCard.

The `close [document {in|with}] <i>application</i>` command closes the named running document, application,  or desk accessory.   (The words `in` and `with` are synonymous.)

Note: This command works only with Apple event-aware applications running under System 7 on the same Macintosh as HyperCard.

If the document or application isn’t running, `the result` is set to `No such document` or `No such application`  as appropriate.

The form close application sends a quit Apple event, while the form  `close document {in|with} <i>application</i>`  sends a `clos` Apple event.

All Apple event-aware applications support the `quit` Apple event, but they don’t all support `clos`.

The `close <i>externalWindow</i>` command closes an external window—a palette or other window displayed by an external command or external function—and removes it from the window list.

Thus you can’t `show` an external window once you’ve closed it; you’ll have to create a new one using its external command or external function.

The `close card window` command closes the frontmost stack if at least two stacks are open.

HyperCard also sends the `close` command to the current card when  the user clicks the close box of  the card window.  You can handle the message as follows:

```
on close
  <i>statements</i>
end close
```

## Examples

```
close printing

close "MicroSoft Works"
close "Alarm Clock"

close file "My Data File"
close file "Simonides:Help Text"
close file theOpenFile

close window "Script of stack My HD:Home" -- external window
close window "Navigator" -- external window

close card window
close window "Home"
```

## Placeholders

[embed:HelpExtras/Placeholders/fileName.md]

[embed:HelpExtras/Placeholders/application.md]

[embed:HelpExtras/Placeholders/externalWindow.md]

[embed:HelpExtras/Placeholders/statements.md]

## Related Topics

* [Commands sent automatically](/HyperTalkReference/systemmessages/Commands-sent-automatically)
* [hide](/HyperTalkReference/commands/hide)
* [moveWindow](/HyperTalkReference/systemmessages/moveWindow)
* [open file](/HyperTalkReference/commands/open-file)
* [open printing](/HyperTalkReference/commands/open-printing)
* [open report printing](/HyperTalkReference/commands/open-report-printing)
* [print](/HyperTalkReference/commands/print)
* [read](/HyperTalkReference/commands/read)
* [reset](/HyperTalkReference/commands/reset)
* [sizeWindow](/HyperTalkReference/systemmessages/sizeWindow)
* [Where messages are sent initially](/HyperTalkReference/systemmessages/Where-messages-are-sent-initially)
* [write](/HyperTalkReference/commands/write)
