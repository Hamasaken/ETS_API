---
title: Stat
draft: false
tags:
 - ScriptType
---
# Stat : [[Any]]

A Stat is a single numeric attribute of a [[Character]], such as Strength, Health or Speed. Its final `value` is worked out from three parts: a base number, a flat modifier added on top, and a multiplier. Effects change a stat by adjusting those parts — nudging the base, adding a temporary bonus, or applying a multiplier — rather than setting the final value directly.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| value | [[Int]] | True | The final value after base, modifier and multiplier combine. |
| base | [[Int]] | False | The base number before modifiers; changing it is permanent. |
| modifier | [[Int]] | True | The total flat bonus or penalty added on top of the base. |
| multiplier | [[Float]] | True | The multiplier applied to the base value. |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Stat#^addbase876899240\|AddBase()]] | [[Void]] | [[Int]] value | Permanently raises the base number. |
| [[Stat#^removebase244046743\|RemoveBase()]] | [[Void]] | [[Int]] value | Permanently lowers the base number. |
| [[Stat#^add-1873257617\|Add()]] | [[Void]] | [[Int]] value, \[[[String]] source\] | Adds a temporary flat bonus. |
| [[Stat#^remove-321068522\|Remove()]] | [[Void]] | [[Int]] value, \[[[String]] source\] | Removes a matching flat bonus. |
| [[Stat#^applymulti-2089238476\|ApplyMulti()]] | [[Void]] | [[Float]] multiplier, \[[[String]] source\] | Applies a multiplier; several stack by multiplying. |
| [[Stat#^removemulti-1772167366\|RemoveMulti()]] | [[Void]] | [[Float]] multiplier, \[[[String]] source\] | Removes a matching multiplier. |



### AddBase ([[Int]] value) : [[Void]]

^addbase876899240

Permanently raises the stat's base number by the given amount. This is a lasting change, unlike the temporary bonus from [[Stat#^add-1873257617\|Add()]].

> [!Abstract]+ Parameters
> 1. `value` How much to add to the base number.

### RemoveBase ([[Int]] value) : [[Void]]

^removebase244046743

Permanently lowers the stat's base number by the given amount. The base will not drop below the stat's minimum.

> [!Abstract]+ Parameters
> 1. `value` How much to subtract from the base number.

### Add ([[Int]] value, \[[[String]] source\]) : [[Void]]

^add-1873257617

Adds a flat bonus on top of the stat's base value — for example a temporary +2 from a buff. Take it back off later with the matching [[Stat#^remove-321068522\|Remove()]].

> [!Abstract]+ Parameters
> 1. `value` The bonus to add (use a negative number for a penalty).
> 2. `source` An optional label naming where the bonus came from, so it can be told apart from others and removed exactly.

### Remove ([[Int]] value, \[[[String]] source\]) : [[Void]]

^remove-321068522

Removes a flat bonus that was added with [[Stat#^add-1873257617\|Add()]], undoing it. Usually called when a temporary effect ends.

> [!Abstract]+ Parameters
> 1. `value` The bonus to remove (matching the one that was added).
> 2. `source` The label the bonus was added with; only a bonus matching both value and source is removed.

### ApplyMulti ([[Float]] multiplier, \[[[String]] source\]) : [[Void]]

^applymulti-2089238476

Multiplies the stat's value by the given amount — for example 1.5 for +50%, or 0.5 to halve it. Several multipliers stack by multiplying together (two 1.5s make 2.25), and a 0 zeroes the stat out entirely until it is removed. Undo it later with the matching [[Stat#^removemulti-1772167366\|RemoveMulti()]].

> [!Abstract]+ Parameters
> 1. `multiplier` The amount to multiply the stat by.
> 2. `source` An optional label naming where the multiplier came from, so it can be told apart from others and removed exactly.

### RemoveMulti ([[Float]] multiplier, \[[[String]] source\]) : [[Void]]

^removemulti-1772167366

Undoes a multiplier that was applied with [[Stat#^applymulti-2089238476\|ApplyMulti()]], taking it back out of the stack. Usually called when a temporary effect ends.

> [!Abstract]+ Parameters
> 1. `multiplier` The multiplier to remove (matching the one that was applied).
> 2. `source` The label the multiplier was applied with; only a multiplier matching both value and source is removed.

