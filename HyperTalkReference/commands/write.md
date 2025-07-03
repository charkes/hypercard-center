---
title: write
card_id: 51002
---

# write

```
write [ph:text] to file [ph:fileName] ¬
 [at {eof|end|[-][ph:integer]]}
```

The `write` command copies text to a file. You must have already opened the file with the `open file` command, and you should close it when writing is completed with the `close file` command.  

The first `write` command after opening a file begins at the start of a file unless you use the `at [ph:integer]` option, with `[ph:integer]` as the character position within the file where writing is to begin.

The `-[ph:integer]` option begins writing at `[ph:integer]` characters from the file's end.

<b>Warning:</b> HyperCard <b>does not ask</b> if you want to write over existing text.

Subsequent `write` commands append text to the file’s contents after the last character written until you close the file.

Note: You must provide the full path name of the file if it’s not at the same directory level as HyperCard.

## Examples

```
write "Hello" to file "My Data"

write field 1 & return & field 2 to file "My Data"
write someStuff to file "My File" at -15

on writeData theData
  ask file "Write to what text file?" with "Untitled"
  if it is empty then exit writeData
  put it into theFileName
  open file theFileName
  write theData to file theFileName
  close file theFileName
end writeData
```

## Related Topics

* [close](/HyperTalkReference/commands/close)
* [open file](/HyperTalkReference/commands/open-file)
* [print](/HyperTalkReference/commands/print)
* [read](/HyperTalkReference/commands/read)
