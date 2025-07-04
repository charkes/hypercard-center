---
title: showPict
card_id: 82724
---

# showPict

```
set [the] showPict of [ph:card] to [ph:trueOrFalse]
set [the] showPict of [ph:bkgnd] to [ph:trueOrFalse]
```

The `showPict` property returns or sets whether HyperCard shows any graphics or paint text for a card and background. The default value is true, meaning that all graphics and paint appear.

When a card picture or background picture is hidden and you try to use a Paint tool on it or paste a picture onto it, a dialog box appears asking if you want to make the picture visible. Clicking OK shows the picture; clicking the Cancel button cancels the action.

If you draw on a hidden picture from a handler, you do not get the dialog box, and whatever you draw will appear after you set `showPict` to true. 

## Examples

```
set showPict of this card to true
set showPict of prev background to true
set showPict of card id 23484 to false

-- Get the current status of showPict:
get showPict of first card
get showPict of myBackgroundVariable
```

## Demo Script

```
on flashPicture
   -- Flash the background picture 3 times:
   repeat 6 times
      set <b>showPict </b>of this bkgnd to not the <b>showPict </b>of this bkgnd
   end repeat
end flashPicture
```

## Related Topics

* [hide](/HyperTalkReference/commands/hide)
* [show](/HyperTalkReference/commands/show)
* [visible](/HyperTalkReference/properties/visible)
