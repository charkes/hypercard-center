---
title: open file
card_id: 41996
---

# open file

<code>open file [ph:fileName</code>]

The <code>open file</code> command opens the specified file so that you can read data from it and write to it. Usually, the file is an ASCII text file opened to allow importing or exporting text. If the file doesn’t exist, HyperCard creates it.

Use the <code>close file</code> command to close files after you’ve opened them.

Note: You must provide the full path name of the file if it’s not at the same directory level as HyperCard. 

 If HyperCard has problems opening the specified file, it sets <code>the result</code> as follows:<code>  </code> Nonexistent file that can't be created: <code><pre>
Can't create that file.
</pre></code>

Existing file already open: <code><pre>
File is already open.
</pre></code>

Other error opening file: <code>Can't open that file.</code>



## Examples

```
open file "My Data"

answer file "Import text from:" of type text
put it into theFile
if theFile is not empty then
  open file theFile
  ... -- process the file
  close file theFile
end if
```

## Related Topics

* [close](/HyperTalkReference/commands/close)
* [open](/HyperTalkReference/commands/open)
* [print](/HyperTalkReference/commands/print)
* [read](/HyperTalkReference/commands/read)
* [write](/HyperTalkReference/commands/write)
