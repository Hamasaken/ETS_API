---
title: Targeting
draft: false
tags:
 - ScriptObject
---

Description goes here.

## Variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| tileTargeting | [[Bool]] | False |  |
| amount | [[Int]] | False |  |
| acceptLess | [[Bool]] | False |  |
| description | [[String]] | False |  |
| rangeMin | [[Int]] | False |  |
| rangeMax | [[Int]] | False |  |
| area | [[Int]] | False |  |
| overlap | [[Bool]] | False |  |

## Functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Targeting#^cantarget\|CanTarget()]] | [[Bool]] | [[Unit]] u, [[Unit]] t |  |
| [[Targeting#^cantargett\|CanTargetT()]] | [[Bool]] | [[Unit]] u, [[Tile]] t |  |
| [[Targeting#^canaoe\|CanAoe()]] | [[Bool]] | [[Unit]] u, [[Unit]] t |  |
| [[Targeting#^canaoet\|CanAoeT()]] | [[Bool]] | [[Unit]] u, [[Tile]] t |  |

### CanTarget ([[Unit]] u, [[Unit]] t) : [[Bool]]

^cantarget

Description goes here.

> [!Abstract]+ Parameters
> 1. `u` This is a parameter.
> 2. `t` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### CanTargetT ([[Unit]] u, [[Tile]] t) : [[Bool]]

^cantargett

Description goes here.

> [!Abstract]+ Parameters
> 1. `u` This is a parameter.
> 2. `t` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### CanAoe ([[Unit]] u, [[Unit]] t) : [[Bool]]

^canaoe

Description goes here.

> [!Abstract]+ Parameters
> 1. `u` This is a parameter.
> 2. `t` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### CanAoeT ([[Unit]] u, [[Tile]] t) : [[Bool]]

^canaoet

Description goes here.

> [!Abstract]+ Parameters
> 1. `u` This is a parameter.
> 2. `t` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

