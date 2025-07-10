---
title: MathUtil
draft: false
tags:
 - ScriptObject
---

Can be used in any script through the global alias "Math".

Example:
```js
var a:Int = 5;
var b:Float = 1.3;
var c:Int = 0;

// Convert result of the operation to an int before storing it in variable "c"
c = Math.ToInt(a * b);

// The following will crash, since a float value can't be applied to an integer variable
c = a * b;
```


## Variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[MathUtil#^toint\|ToInt()]] | [[Int]] | [[Any]] number |  |
| [[MathUtil#^tofloat\|ToFloat()]] | [[Float]] | [[Any]] number |  |

### ToInt ([[Any]] number) : [[Int]]

^toint

Description goes here.

> [!Abstract]+ Parameters
> 1. `number` This is a parameter.

> [!Success]+ Return value
> Returns a [[Int]].

### ToFloat ([[Any]] number) : [[Float]]

^tofloat

Description goes here.

> [!Abstract]+ Parameters
> 1. `number` This is a parameter.

> [!Success]+ Return value
> Returns a [[Float]].

