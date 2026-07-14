---
title: Int
draft: false
tags:
 - ScriptType
---
# Int : [[Any]]

An Int is a whole number, with no decimal part — like 0, 1, 5 or -3. Ints are used for anything counted in whole units: action points, tile distances, item quantities, the number of targets an ability hits, and so on. When you need fractions, use a [[Float]] instead.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Int#^parse-114875254\|Parse()]] | [[Int]] | [[String]] input | Reads a whole number out of text. |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |



### Parse ([[String]] input) : [[Int]]

^parse-114875254

Turns a piece of text into a whole number, for example when a value was written or stored as text. The text must be a valid whole number; anything else causes an error.

> [!Abstract]+ Parameters
> 1. `input` The text to read the whole number from.

> [!Success]+ Return value
> Returns the whole number the text represents.

