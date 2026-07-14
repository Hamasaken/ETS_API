---
title: Bool
draft: false
tags:
 - ScriptType
---
# Bool : [[Any]]

A Bool is a simple true/false (yes/no) value. Bools are what conditions evaluate to — whether an ability can target a unit, whether a status is still active, whether a tile is walkable, and so on. Anywhere a script asks a yes-or-no question, the answer is a Bool.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Bool#^parse-114875254\|Parse()]] | [[Bool]] | [[String]] input | Reads a true/false value out of text. |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |



### Parse ([[String]] input) : [[Bool]]

^parse-114875254

Turns a piece of text into a true/false value, for example when a value was written or stored as text. The text must clearly say true or false; anything it can't recognise causes an error.

> [!Abstract]+ Parameters
> 1. `input` The text to read the true/false value from.

> [!Success]+ Return value
> Returns the true/false value the text represents.

