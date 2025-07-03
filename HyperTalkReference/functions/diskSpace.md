---
title: diskSpace
card_id: 55302
---

# diskSpace

```
the diskSpace [of disk [ph:diskName]]
```

Value returned: a positive integer equal to the number of bytes of free space on the disk that contains the current stack or of the disk whose name appears in [ph:<code>diskName </code>](assuming [ph:<code>diskName </code>]is a mounted volume).

## Examples

```
if (the diskSpace div 1024) < 5000 then
   answer "Your disk is getting full."  
end if

if diskSpace of disk "Outside" > size of this stack then do fld 5

get the diskSpace of disk "Major Projects"
```

## Demo Script

```
on reportDiskSpace
  set the numberFormat to "0.0"
  answer "The amount of space left on the disk named" && diskName() && ¬
  "is" && the diskSpace / 1024000 && "megabytes."
end reportDiskSpace

function diskName longStackName
  if longStackName is empty
  then put the long name of this stack into longStackName
  delete char 1 to 7 of longStackName -- remove “stack "”
  return char 1 to offset(":",longStackName) - 1 of longStackName
end diskName
```

## Related Topics

* [freeSize](/HyperTalkReference/properties/freeSize)
* [size](/HyperTalkReference/properties/size)
