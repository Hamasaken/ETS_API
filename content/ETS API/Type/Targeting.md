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
| u | [[Character]] | False |  |
| t | [[Character]] | False |  |
| amount | [[Int]] | False |  |
| acceptLess | [[Bool]] | False |  |
| description | [[String]] | False |  |
| rangeMin | [[Int]] | False |  |
| rangeMax | [[Int]] | False |  |
| area | [[Int]] | False |  |
| tileTargeting | [[Bool]] | False |  |

## Functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Targeting#^cantarget\|CanTarget()]] | [[Bool]] | [[Character]] u, [[Character]] t |  |
| [[Targeting#^cantargett\|CanTargetT()]] | [[Bool]] | [[Character]] u, [[Tile]] t |  |

### CanTarget ([[Character]] u, [[Character]] t) : [[Bool]]

^cantarget

Description goes here.

> [!Abstract]+ Parameters
> 1. `u` This is a parameter.
> 2. `t` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### CanTargetT ([[Character]] u, [[Tile]] t) : [[Bool]]

^cantargett

Description goes here.

> [!Abstract]+ Parameters
> 1. `u` This is a parameter.
> 2. `t` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

