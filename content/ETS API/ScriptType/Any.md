---
title: Any
draft: false
tags:
 - ScriptType
---
# Any

Any means "a value of any type". It's the common ancestor of every other type in the language, so wherever something is described as an Any it can hold a number, some text, a unit, a list — anything at all. You'll see Any used where a function accepts or returns a value whose exact type isn't fixed in advance, such as the items stored in a [[List]].

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Any#^tostring-1865520797\|ToString()]] | [[String]] |  | Turns the value into readable text. |



### ToString () : [[String]]

^tostring-1865520797

Produces a readable text version of the value, handy for building messages or for logging. Text is shown in quotes, lists and dictionaries are laid out neatly, and an empty value becomes the word `null`.

> [!Success]+ Return value
> Returns the value written out as text.

