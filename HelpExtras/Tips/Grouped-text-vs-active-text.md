---
title: Grouped text vs. active text
card_id: 34776
---

### Grouped text vs. active text

In HyperCard, all text can be <b>active text </b>(text that does something when the user clicks it), but you have to write a HyperTalk handler to make something happen.

By default, HyperCard groups text as words or lines. You can get the word or the line that the user clicked with the HyperTalk functions `the clickChunk`, `the selectedLine`, `the clickLine`, or `the clickText`. (For more information, see the HyperTalk Reference stack.) You use the <b>Group text</b> style to override HyperCard’s default grouping of text.

HyperCard treats the entire run of grouped text as the text clicked by the user. For example, by grouping the phrase `background button` you could look up the entire string in a glossary, as opposed to looking up just the word `background` or the word `button`.

You can choose whether to make the Group style visible to the user (with a thick gray underline) by using the commands `show groups` and `hide groups`.

<b>Important</b>: Grouping text does not automatically make it active text—you still have to write a handler to determine what text the user clicked and then to perform some action.
