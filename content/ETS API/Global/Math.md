---
title: Math
draft: false
tags:
 - Scope
---
# Math

Can be used in any script through the global alias "Math".

Example:
```js
var a:Int = 5;
var b:Float = 1.3;
var c:Int = 0;

// Convert result of the operation to an int before storing it in variable "c"
c = Math.ToInt(a * b);

// The following will crash, since a float value can't be stored in an integer variable
c = a * b;
```


## Script variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |


## Script functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Math#^toint-493137953\|ToInt()]] | [[Int]] | [[Any]] number |  |
| [[Math#^tofloat-159462994\|ToFloat()]] | [[Float]] | [[Any]] number |  |


### ToInt ([[Any]] number) : [[Int]]

^toint-493137953

This is a function.

> [!Abstract]+ Parameters
> 1. `number` This is a parameter.

> [!Success]+ Return value
> Returns a [[Int]].

### ToFloat ([[Any]] number) : [[Float]]

^tofloat-159462994

This is a function.

> [!Abstract]+ Parameters
> 1. `number` This is a parameter.

> [!Success]+ Return value
> Returns a [[Float]].

