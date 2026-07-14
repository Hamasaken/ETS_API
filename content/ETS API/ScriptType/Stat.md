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
| [[Stat#^add-2138638215\|Add()]] | [[Void]] | [[Int]] value | Adds a flat bonus (undo with Remove). |
| [[Stat#^remove-980188942\|Remove()]] | [[Void]] | [[Int]] value | Removes a flat bonus added with Add. |
| [[Stat#^applymulti1595172628\|ApplyMulti()]] | [[Void]] | [[Float]] multiplier | Applies a multiplier to the stat. |
| [[Stat#^removemulti-888451250\|RemoveMulti()]] | [[Void]] | [[Float]] multiplier | Undoes a multiplier applied with ApplyMulti. |



### AddBase ([[Int]] value) : [[Void]]

^addbase876899240

Permanently raises the stat's base number by the given amount. This is a lasting change, unlike the temporary bonus from [[Stat#^add-2138638215\|Add()]].

> [!Abstract]+ Parameters
> 1. `value` How much to add to the base number.

### RemoveBase ([[Int]] value) : [[Void]]

^removebase244046743

Permanently lowers the stat's base number by the given amount. The base will not drop below the stat's minimum.

> [!Abstract]+ Parameters
> 1. `value` How much to subtract from the base number.

### Add ([[Int]] value) : [[Void]]

^add-2138638215

Adds a flat bonus on top of the stat's base value — for example a temporary +2 from a buff. Take it back off later with the matching [[Stat#^remove-980188942\|Remove()]].

> [!Abstract]+ Parameters
> 1. `value` The bonus to add (use a negative number for a penalty).

### Remove ([[Int]] value) : [[Void]]

^remove-980188942

Removes a flat bonus that was added with [[Stat#^add-2138638215\|Add()]], undoing it. Usually called when a temporary effect ends.

> [!Abstract]+ Parameters
> 1. `value` The bonus to remove (matching the one that was added).

### ApplyMulti ([[Float]] multiplier) : [[Void]]

^applymulti1595172628

Multiplies the stat's value by the given amount — for example 1.5 for +50%, or 0.5 to halve it. Undo it later with the matching [[Stat#^removemulti-888451250\|RemoveMulti()]].

> [!Abstract]+ Parameters
> 1. `multiplier` The amount to multiply the stat by.

### RemoveMulti ([[Float]] multiplier) : [[Void]]

^removemulti-888451250

Undoes a multiplier that was applied with [[Stat#^applymulti1595172628\|ApplyMulti()]], dividing it back out. Usually called when a temporary effect ends.

> [!Abstract]+ Parameters
> 1. `multiplier` The multiplier to remove (matching the one that was applied).

