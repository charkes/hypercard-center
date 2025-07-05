---
title: Find and match
card_id: 21415
---

### Find and match

* `find` looks for the first card that contains everything between the quotation marks, even if the words are in a different order or in different fields. To find an exact match, use `find whole`. If HyperCard can’t find the text, it beeps (or the menu bar flashes).

* `find` ignores case and diacritical marks. The following phrases are equivalent:

```
 apple Cømpüter
 apple computer
 Apple COMPUTER
```

To respect diacritical marks, ligatures, and other international characters, use `find [[ph:modifier]] international`.

* To restrict the search to a specific field, use the name, number, or ID of the field. The following examples show what you might type into the Message box to restrict the search:

```
find "Duffy" in card field 1
find "Kat" in background field "Name"
find "Gualala" in field id 3748
```

* To use text from any field on the current card for the `find` string: Press     Command-F to display the `find` command; then Command-drag  across text.

* Include enough text in the `find` string to distinguish your target from other text in the stack. This prevents HyperCard from taking you to cards that don’t actually have what you’re looking for.  

* Specify your target as strings with multiples of three characters (not counting spaces). HyperCard searches faster for three-character strings.
