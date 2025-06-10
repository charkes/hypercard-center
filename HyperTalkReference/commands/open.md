---
title: open
card_id: 41778
---

# open

<code><pre>
open [ph:application]
open [ph:fileName] with [ph:application]
</pre></code>

The <code>open</code> command launches another application program or opens a document with another application from within HyperCard. You must provide the full path names for the files if they’re not at the same directory level as HyperCard.

Under the Finder in System 6, HyperCard sends the <code>suspend</code> system message to the current card before turning over control to the application.

If HyperCard can’t find the document or application, it displays a directory dialog box and asks the user to find it. HyperCard also sets <code>the result</code> to <code>Cancel</code> if the user clicks Cancel in the dialog box. Otherwise, it sets <code>the result</code> to <code>empty</code>.

If HyperCard has problems opening the specified application (for example, there’s not enough memory), it sets <code>the result</code> to <code>"Couldn't open that application."</code>

## Examples

```
open "TeachText"
open "Read Me" with "Teach Text"
open "the document you want" with "the application" -- invoke dialog box

answer file "Start what application?" of type application
if it is not empty then open it
```

## Demo Script

<code><pre>
on mouseUp
  -- this demo only works with System 7
  if not systemSeven() then exit mouseUp
  -- asks the user for an application
  put askForApplication() into appName
  if appName is empty then exit mouseUp
  <b>open</b> appName -- open the selected application
  wait 5
  <b>open</b> the long name of HyperCard -- bring HyperCard to front
  wait 30
  close appName -- close the just opened application
end mouseUp

function askForApplication
  answer file "Select an application to open:" of type "APPL"
  if it is empty then return empty
  if it is the long name of HyperCard then
    -- the user selected the current running HyperCard
    answer "Try selecting an application other than HyperCard."
    return askForApplication() -- recursion
  else return it
end askForApplication

function systemSeven
  return the systemVersion ≥ 7.0
end systemSeven
</pre></code>

## Related Topics

* [open file](/HyperTalkReference/commands/open-file)
