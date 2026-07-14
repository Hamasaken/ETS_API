---
title: String
draft: false
tags:
 - ScriptType
---
# String : [[Any]]

A String is a piece of text — anything from a single word to a whole sentence. Strings hold names, ids, and messages: a character's name, an ability's id, a line of dialogue, or a label a script builds up and shows to the player. Text you write directly in a script goes inside quotes, like `"Hello"`.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| Length | [[Int]] | True | How many characters the text contains. |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[String#^contains-2139094480\|Contains()]] | [[Bool]] | [[String]] value | True if the text contains this snippet anywhere. |
| [[String#^startswith-2031788726\|StartsWith()]] | [[Bool]] | [[String]] value | True if the text begins with this snippet. |
| [[String#^endswith-123236167\|EndsWith()]] | [[Bool]] | [[String]] value | True if the text ends with this snippet. |
| [[String#^indexof1066720368\|IndexOf()]] | [[Int]] | [[String]] value | Position where the snippet first appears. |
| [[String#^substring-1051558006\|Substring()]] | [[String]] | [[Int]] startIndex, \[[[Int]] length\] | Cuts out part of the text. |
| [[String#^replace1456680773\|Replace()]] | [[String]] | [[String]] oldValue, [[String]] newValue | Swaps every copy of one snippet for another. |
| [[String#^split-1533391272\|Split()]] | [[List]]<[[String]]> | [[String]] separator, [[Int]] count | Breaks the text into a list of pieces. |



### Contains ([[String]] value) : [[Bool]]

^contains-2139094480

Checks whether this text contains the given snippet anywhere inside it. The match is exact, including upper- and lower-case.

> [!Abstract]+ Parameters
> 1. `value` The snippet of text to look for.

> [!Success]+ Return value
> Returns true if the snippet appears somewhere in the text.

### StartsWith ([[String]] value) : [[Bool]]

^startswith-2031788726

Checks whether this text begins with the given snippet. Useful for spotting ids that share a common prefix.

> [!Abstract]+ Parameters
> 1. `value` The snippet the text should start with.

> [!Success]+ Return value
> Returns true if the text starts with the snippet.

### EndsWith ([[String]] value) : [[Bool]]

^endswith-123236167

Checks whether this text ends with the given snippet. Useful for spotting file extensions or ids that share a common suffix.

> [!Abstract]+ Parameters
> 1. `value` The snippet the text should end with.

> [!Success]+ Return value
> Returns true if the text ends with the snippet.

### IndexOf ([[String]] value) : [[Int]]

^indexof1066720368

Finds where the given snippet first appears in the text and returns its position. Positions are counted from 0, so the first character is at position 0. Returns -1 when the snippet isn't found at all.

> [!Abstract]+ Parameters
> 1. `value` The snippet of text to search for.

> [!Success]+ Return value
> Returns the position of the first match, or -1 if the snippet is not present.

### Substring ([[Int]] startIndex, \[[[Int]] length\]) : [[String]]

^substring-1051558006

Cuts out and returns a portion of the text, starting at the given position (counted from 0). If you give a length, that many characters are taken; if you leave it out, everything from the start position to the end of the text is taken.

> [!Abstract]+ Parameters
> 1. `startIndex` Where to start cutting, counted from 0 (the first character).
> 2. `length` How many characters to take. Leave out to take the rest of the text.

> [!Success]+ Return value
> Returns the portion of the text you asked for.

### Replace ([[String]] oldValue, [[String]] newValue) : [[String]]

^replace1456680773

Returns a copy of the text with every occurrence of one snippet swapped out for another. The original text is left unchanged.

> [!Abstract]+ Parameters
> 1. `oldValue` The snippet to look for and replace.
> 2. `newValue` The snippet to put in its place.

> [!Success]+ Return value
> Returns a new piece of text with the replacements made.

### Split ([[String]] separator, [[Int]] count) : [[List]]<[[String]]>

^split-1533391272

Breaks the text into a [[List]] of smaller pieces, cutting it wherever the separator appears. The separators themselves are removed. For example, splitting `"a,b,c"` on `","` gives the three pieces `"a"`, `"b"` and `"c"`.

> [!Example]+ Example
> Split an id like `"fire_bolt"` into its parts:
> ```js
> "fire_bolt".Split("_", 0)
> ```

> [!Abstract]+ Parameters
> 1. `separator` The snippet to cut the text at.
> 2. `count` The most pieces to produce. Use 0 for no limit.

> [!Success]+ Return value
> Returns the list of pieces the text was split into.

