---
title: read
card_id: 45683
---

# read

<code><pre>
read from file [ph:fileName] [at [-] ¬
[ph:integer]] {for [ph:posInteger] |until [ph:char]}
</pre></code>

The <code>read</code> command reads data from a file. (You must have already opened the file with the <code>open file</code> command.) <code> Read </code>places the data into the local variable<code> it</code>.

Reading of a newly opened file starts from the beginning of the  file, or optionally  <code>at </code>character [ph:<code>integer]. </code>If you use the form <code>at -[ph:integer</code>], reading starts at [ph:<code>integer] </code>characters from the end of 

the file. Subsequent reads continue from the last point read.<code>

Read </code>continues until it has read the specified number of characters or it reaches the named ASCII character (which can be specified as a constant: <code> colon, comma, end</code>, <code>eof</code>,<code> formfeed</code>,<code> quote</code>,<code> return</code>,<code> space</code>,<code></code> or<code> tab</code>).

All characters count as data, including return characters at the end of lines, spaces, and tab characters. 


## Examples

```
read from file "Data" until Z -- read until first Z  
read from file "Data" until tab  
read from file "Data" until return -- read one line
read from file "Data" until end -- read until the end of the file
read from file "Data" for 100 -- read 100 bytes
read from file "Data" at 200 for 100 -- read 100 bytes ¬
                starting at the 200th character in the file
read from file "Data" at -200 for 100 -- read 100 bytes ¬
                starting at the 200th character from the end of the file
 
read from file "My Data"
-- This function asks for the name of a text file and reads it.
-- You might use it as follows: 

-- put readFile() into myInfo

-- Note that variables can hold unlimited amounts of information
-- while fields can only hold 30k.

function readFile
  answer file "Read what text file?" of type text
  if (it is empty) or (it is "Cancel") then return empty
  put it into theFileName
  open file theFileName
  repeat forever
    read from file theFileName for 16384
    if it is empty then exit repeat
    put it after theData
  end repeat
  close file theFileName
  return theData
end readFile
```

## Related Topics

* [close](/HyperTalkReference/commands/close)
* [open](/HyperTalkReference/commands/open)
* [open file](/HyperTalkReference/commands/open-file)
* [print](/HyperTalkReference/commands/print)
* [write](/HyperTalkReference/commands/write)
