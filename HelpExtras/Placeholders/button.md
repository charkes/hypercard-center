### button

<b>HyperTalk Definition</b>

An expression that identifies a button by name, number, or id, using one of the following forms:

```
[card] button id [ph:posInteger] [of [ph:card]]
[card] button [ph:text] [of [ph:card]] -- name
[card] button [ph:posInteger] [of [ph:card]]
[ph:ordinal] [card] button [of [ph:card]]

bkgnd button id [ph:posInteger] [of [ph:card]]
bkgnd button [ph:text] [of [ph:card]] -- name
bkgnd button [ph:posInteger] [of [ph:card]]
[ph:ordinal] bkgnd button [of [ph:card]]
```

For example:

```
card button id 3894
card button "Return"
card button 1
first card button
bkgnd button 2 of card 2
last bkgnd button
```

When used inside a button script: `me`

When a button receives a message: `[the] target`

A button can also be referred to as a [ph:part] when you’re talking about its position among all buttons and fields within the same card or background.

<b>AppleScript Definition</b>

An expression that identifies a button by name, number, or id, using the same forms as HyperTalk except that “background” must be used in place of “bkgnd”.
