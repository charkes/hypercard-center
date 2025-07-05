---
title: Shortcuts for scripting
card_id: 5960
---

### Shortcuts for scripting

You can use the following shortcuts while you’re editing scripts in a script window (in addition to the Command-key equivalents in the menus):

* To indicate a comment, use two hyphens: `--`

* To wrap a line without inserting a return character so that HyperCard still treats it as a single statement, press Option-Return (shown by the character “¬” in scripts).

* To reformat a script, press Tab. (Look for end statements that don’t line up properly to indicate places you’ve made syntax errors.)

* To select a whole line, triple-click.

* To select the text between two quotation marks, double-click a quotation mark.

* To select the text between two parentheses, double-click the left parenthesis.

* To move the cursor to the beginning of the current line, press Command-Left Arrow.

* To move the cursor to the end of the current line, press Command-Right Arrow.

* To move the cursor to the beginning of the script, press Command-Up Arrow.

* To move the cursor to the end of the script, press Command-Down Arrow.

* To close a card script, press Command-Option-C.

* To close a background script, press Command-Option-B.

* To close a stack script, press Command-Option-S.

* To close the current script window, press Command-Option, and click.

* To save your changes and close the current script window, press Enter.

* To abandon changes and close the current script window, press Command-. (Command-period).

* To close all open script windows, hold down the Option key, and choose Close All Scripts from the File menu (or hold down the Option key, and click the close box of the active script window).

* To place or remove a temporary checkpoint, hold down the Option key, and click. You can set up to 16 temporary checkpoints per script in up to 32 scripts. They arenot  saved with the script.

* To remove all temporary checkpoints in a script, hold down the Shift key and the Option key and click an existing checkpoint.

* To enter the debugger while a script is running, even if you haven’t set a checkpoint, press Command-Option-. (Command-Option-period).

* To set where the script windows will appear on screen, place a `[ph:rect]` into each line of the global variable `scriptWindowRects`. Line 1 determines where the first script window will appear, line 2 the second, and so on.
