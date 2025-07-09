---
title: String
draft: false
tags:
 - ScriptObject
---

Description goes here.

## Variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[String#^length\|Length()]] | [[Int]] |  |  |
| [[String#^contains\|Contains()]] | [[Bool]] | [[String]] value |  |
| [[String#^startswith\|StartsWith()]] | [[Bool]] | [[String]] value |  |
| [[String#^endswith\|EndsWith()]] | [[Bool]] | [[String]] value |  |
| [[String#^indexof\|IndexOf()]] | [[Int]] | [[String]] value |  |
| [[String#^substring\|Substring()]] | [[String]] | [[Int]] startIndex, [[Int]] length |  |
| [[String#^replace\|Replace()]] | [[String]] | [[String]] oldValue, [[String]] newValue |  |
| [[String#^split\|Split()]] | [[List]]<[[String]]> | [[String]] separator, [[Int]] count |  |

### Length () : [[Int]]

^length

Gets the length of the string.

> [!Success]+ Return value
> Returns an [[Int]] representing the total amount of characters in the string.

### Contains ([[String]] value) : [[Bool]]

^contains

Checks whether this string contains another string value.

> [!Abstract]+ Parameters
> 1. `value` The string to search for.

> [!Success]+ Return value
> Returns true if the value is found, otherwise false.

### StartsWith ([[String]] value) : [[Bool]]

^startswith

Description goes here.

> [!Abstract]+ Parameters
> 1. `value` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### EndsWith ([[String]] value) : [[Bool]]

^endswith

Description goes here.

> [!Abstract]+ Parameters
> 1. `value` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### IndexOf ([[String]] value) : [[Int]]

^indexof

Description goes here.

> [!Abstract]+ Parameters
> 1. `value` This is a parameter.

> [!Success]+ Return value
> Returns a [[Int]].

### Substring ([[Int]] startIndex, [[Int]] length) : [[String]]

^substring

Description goes here.

> [!Abstract]+ Parameters
> 1. `startIndex` This is a parameter.
> 2. `length` This is a parameter.

> [!Success]+ Return value
> Returns a [[String]].

### Replace ([[String]] oldValue, [[String]] newValue) : [[String]]

^replace

Description goes here.

> [!Abstract]+ Parameters
> 1. `oldValue` This is a parameter.
> 2. `newValue` This is a parameter.

> [!Success]+ Return value
> Returns a [[String]].

### Split ([[String]] separator, [[Int]] count) : [[List]]<[[String]]>

^split

Description goes here.

> [!Abstract]+ Parameters
> 1. `separator` This is a parameter.
> 2. `count` This is a parameter.

> [!Success]+ Return value
> Returns a [[ETS API/Type/List]]<[[String]]>.

