---
title: Random
draft: false
tags:
 - Scope
---
# Random

Can be used in any script through the global alias "Random".

Example:
```js
// Will set 'a' to a random integer between 0 and 10 (but not including 10)
var a:Int = Random.Int(0, 10);
```


## Script variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |


## Script functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Random#^int789484612\|Int()]] | [[Int]] | [[Int]] min, [[Int]] max | A random whole number in a range. |
| [[Random#^float1844544593\|Float()]] | [[Float]] |  | A random number from 0 to 1. |
| [[Random#^float-1213602765\|Float()]] | [[Float]] | [[Float]] min, [[Float]] max | A random number in a range. |


### Int ([[Int]] min, [[Int]] max) : [[Int]]

^int789484612

Picks a random whole number from `min` up to `max`. The lowest value is included, but the highest is not — so `Random.Int(0, 10)` gives a number from 0 to 9.

> [!Abstract]+ Parameters
> 1. `min` The lowest value that can be picked (included).
> 2. `max` The upper limit (not included).

> [!Success]+ Return value
> Returns a random whole number in the range.

### Float () : [[Float]]

^float1844544593

Picks a random decimal number between 0 and 1 — handy for percentage chances, for example checking against `Random.Float() < 0.25` for a 25% chance.

> [!Success]+ Return value
> Returns a random number from 0 up to 1.

### Float ([[Float]] min, [[Float]] max) : [[Float]]

^float-1213602765

Picks a random decimal number between `min` and `max`.

> [!Abstract]+ Parameters
> 1. `min` The lowest value that can be picked.
> 2. `max` The highest value that can be picked.

> [!Success]+ Return value
> Returns a random number in the range.

