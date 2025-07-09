---
title: Unit
draft: false
tags:
 - ScriptObject
---

Description goes here.

## Variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| uid | [[String]] | True |  |
| visuals | [[UnitVisuals]] | True |  |
| c | [[Character]] | True |  |
| character | [[Character]] | True |  |
| x | [[Int]] | False |  |
| y | [[Int]] | False |  |
| team | [[Team]] | False |  |

## Functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Unit#^isally\|IsAlly()]] | [[Bool]] | [[Unit]] unit |  |
| [[Unit#^isenemy\|IsEnemy()]] | [[Bool]] | [[Unit]] unit |  |

### IsAlly ([[Unit]] unit) : [[Bool]]

^isally

Description goes here.

> [!Abstract]+ Parameters
> 1. `unit` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### IsEnemy ([[Unit]] unit) : [[Bool]]

^isenemy

Description goes here.

> [!Abstract]+ Parameters
> 1. `unit` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

