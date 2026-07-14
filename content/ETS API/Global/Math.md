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
| [[Math#^toint-493137581\|ToInt()]] | [[Int]] | [[Float]] number | Drops the decimals to give a whole number. |
| [[Math#^tofloat-159462994\|ToFloat()]] | [[Float]] | [[Any]] number | Converts a value to a decimal number. |
| [[Math#^abs-119868498\|Abs()]] | [[Int]] | [[Int]] number | Distance from zero (always positive). |
| [[Math#^abs-119868467\|Abs()]] | [[Float]] | [[Float]] number | Distance from zero (always positive). |
| [[Math#^min-237914991\|Min()]] | [[Int]] | [[Int]] n1, [[Int]] n2 | The smaller of two whole numbers. |
| [[Math#^min-237913999\|Min()]] | [[Float]] | [[Float]] n1, [[Float]] n2 | The smaller of two numbers. |
| [[Math#^max-643150737\|Max()]] | [[Int]] | [[Int]] n1, [[Int]] n2 | The larger of two whole numbers. |
| [[Math#^max-643149745\|Max()]] | [[Float]] | [[Float]] n1, [[Float]] n2 | The larger of two numbers. |
| [[Math#^ceil-969025378\|Ceil()]] | [[Float]] | [[Float]] number | Rounds up to a whole number. |
| [[Math#^floor2105069935\|Floor()]] | [[Float]] | [[Float]] number | Rounds down to a whole number. |
| [[Math#^round-490836947\|Round()]] | [[Float]] | [[Float]] number | Rounds to the nearest whole number. |
| [[Math#^pow1826179999\|Pow()]] | [[Float]] | [[Float]] n1, [[Float]] n2 | One number raised to the power of another. |
| [[Math#^sqrt1305297943\|Sqrt()]] | [[Float]] | [[Float]] number | The square root of a number. |
| [[Math#^acos919608935\|Acos()]] | [[Float]] | [[Float]] number | Inverse cosine (in radians). |
| [[Math#^asin965100120\|Asin()]] | [[Float]] | [[Float]] number | Inverse sine (in radians). |
| [[Math#^atan851221619\|Atan()]] | [[Float]] | [[Float]] number | Inverse tangent (in radians). |
| [[Math#^cos889687930\|Cos()]] | [[Float]] | [[Float]] number | Cosine of an angle (in radians). |
| [[Math#^sin131442951\|Sin()]] | [[Float]] | [[Float]] number | Sine of an angle (in radians). |
| [[Math#^tan-1128650298\|Tan()]] | [[Float]] | [[Float]] number | Tangent of an angle (in radians). |


### ToInt ([[Float]] number) : [[Int]]

^toint-493137581

Converts a decimal number to a whole number by dropping everything after the decimal point. Useful before storing a calculation in an [[Int]] variable.

> [!Abstract]+ Parameters
> 1. `number` The number to convert.

> [!Success]+ Return value
> Returns the whole-number part of the value.

### ToFloat ([[Any]] number) : [[Float]]

^tofloat-159462994

Converts a value to a decimal number, so it can be used in calculations that need fractions.

> [!Abstract]+ Parameters
> 1. `number` The value to convert.

> [!Success]+ Return value
> Returns the value as a decimal number.

### Abs ([[Int]] number) : [[Int]]

^abs-119868498

Gives the size of a whole number ignoring its sign, so -3 and 3 both become 3.

> [!Abstract]+ Parameters
> 1. `number` The whole number to measure.

> [!Success]+ Return value
> Returns the number's distance from zero (never negative).

### Abs ([[Float]] number) : [[Float]]

^abs-119868467

Gives the size of a decimal number ignoring its sign, so -1.5 and 1.5 both become 1.5.

> [!Abstract]+ Parameters
> 1. `number` The number to measure.

> [!Success]+ Return value
> Returns the number's distance from zero (never negative).

### Min ([[Int]] n1, [[Int]] n2) : [[Int]]

^min-237914991

Gives whichever of two whole numbers is smaller.

> [!Abstract]+ Parameters
> 1. `n1` The first number.
> 2. `n2` The second number.

> [!Success]+ Return value
> Returns the smaller of the two numbers.

### Min ([[Float]] n1, [[Float]] n2) : [[Float]]

^min-237913999

Gives whichever of two numbers is smaller.

> [!Abstract]+ Parameters
> 1. `n1` The first number.
> 2. `n2` The second number.

> [!Success]+ Return value
> Returns the smaller of the two numbers.

### Max ([[Int]] n1, [[Int]] n2) : [[Int]]

^max-643150737

Gives whichever of two whole numbers is larger.

> [!Abstract]+ Parameters
> 1. `n1` The first number.
> 2. `n2` The second number.

> [!Success]+ Return value
> Returns the larger of the two numbers.

### Max ([[Float]] n1, [[Float]] n2) : [[Float]]

^max-643149745

Gives whichever of two numbers is larger.

> [!Abstract]+ Parameters
> 1. `n1` The first number.
> 2. `n2` The second number.

> [!Success]+ Return value
> Returns the larger of the two numbers.

### Ceil ([[Float]] number) : [[Float]]

^ceil-969025378

Rounds a number up to the next whole number, so 3.2 becomes 4.

> [!Abstract]+ Parameters
> 1. `number` The number to round up.

> [!Success]+ Return value
> Returns the number rounded up.

### Floor ([[Float]] number) : [[Float]]

^floor2105069935

Rounds a number down to the whole number below it, so 3.8 becomes 3.

> [!Abstract]+ Parameters
> 1. `number` The number to round down.

> [!Success]+ Return value
> Returns the number rounded down.

### Round ([[Float]] number) : [[Float]]

^round-490836947

Rounds a number to the nearest whole number, so 3.5 becomes 4 and 3.2 becomes 3.

> [!Abstract]+ Parameters
> 1. `number` The number to round.

> [!Success]+ Return value
> Returns the number rounded to the nearest whole value.

### Pow ([[Float]] n1, [[Float]] n2) : [[Float]]

^pow1826179999

Raises one number to the power of another — for example `Pow(2, 3)` is 2 × 2 × 2 = 8.

> [!Abstract]+ Parameters
> 1. `n1` The base number.
> 2. `n2` The power to raise it to.

> [!Success]+ Return value
> Returns the base raised to the given power.

### Sqrt ([[Float]] number) : [[Float]]

^sqrt1305297943

Gives the square root of a number — the value that, multiplied by itself, makes the number. For example `Sqrt(9)` is 3.

> [!Abstract]+ Parameters
> 1. `number` The number to take the square root of.

> [!Success]+ Return value
> Returns the square root of the number.

### Acos ([[Float]] number) : [[Float]]

^acos919608935

The inverse cosine: given a cosine value, gives back the angle (in radians) that produced it. An advanced maths function you'll rarely need for everyday scripting.

> [!Abstract]+ Parameters
> 1. `number` A cosine value, between -1 and 1.

> [!Success]+ Return value
> Returns the matching angle in radians.

### Asin ([[Float]] number) : [[Float]]

^asin965100120

The inverse sine: given a sine value, gives back the angle (in radians) that produced it. An advanced maths function you'll rarely need for everyday scripting.

> [!Abstract]+ Parameters
> 1. `number` A sine value, between -1 and 1.

> [!Success]+ Return value
> Returns the matching angle in radians.

### Atan ([[Float]] number) : [[Float]]

^atan851221619

The inverse tangent: given a tangent value, gives back the angle (in radians) that produced it. An advanced maths function you'll rarely need for everyday scripting.

> [!Abstract]+ Parameters
> 1. `number` A tangent value.

> [!Success]+ Return value
> Returns the matching angle in radians.

### Cos ([[Float]] number) : [[Float]]

^cos889687930

The cosine of an angle given in radians. An advanced maths function you'll rarely need for everyday scripting.

> [!Abstract]+ Parameters
> 1. `number` The angle in radians.

> [!Success]+ Return value
> Returns the cosine of the angle.

### Sin ([[Float]] number) : [[Float]]

^sin131442951

The sine of an angle given in radians. An advanced maths function you'll rarely need for everyday scripting.

> [!Abstract]+ Parameters
> 1. `number` The angle in radians.

> [!Success]+ Return value
> Returns the sine of the angle.

### Tan ([[Float]] number) : [[Float]]

^tan-1128650298

The tangent of an angle given in radians. An advanced maths function you'll rarely need for everyday scripting.

> [!Abstract]+ Parameters
> 1. `number` The angle in radians.

> [!Success]+ Return value
> Returns the tangent of the angle.

