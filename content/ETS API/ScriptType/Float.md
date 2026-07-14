---
title: Float
draft: false
tags:
 - ScriptType
---
# Float : [[Any]]

A Float is a number that can have a decimal part — like 0.5, 1.25 or -3.0. Floats are used wherever fractions matter: stat multipliers, hit chances, percentages, and scaling values. When you only ever need whole numbers, use an [[Int]] instead.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Float#^parse-114875254\|Parse()]] | [[Float]] | [[String]] input | Reads a decimal number out of text. |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Float#^toint953923121\|ToInt()]] | [[Int]] |  | Drops the decimals to give a whole number. |



### Parse ([[String]] input) : [[Float]]

^parse-114875254

Turns a piece of text into a decimal number, for example when a value was written or stored as text. The text must be a valid number; anything else causes an error.

> [!Abstract]+ Parameters
> 1. `input` The text to read the number from.

> [!Success]+ Return value
> Returns the number the text represents.

### ToInt () : [[Int]]

^toint953923121

Converts this number to a whole number by dropping everything after the decimal point (rounding toward zero). For example 3.9 becomes 3, and -1.8 becomes -1.

> [!Success]+ Return value
> Returns the whole-number part of this value.

