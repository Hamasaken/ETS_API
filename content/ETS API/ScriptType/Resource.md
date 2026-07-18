---
title: Resource
draft: false
tags:
 - ScriptType
---
# Resource : [[Any]]

A Resource is a pool a [[Character]] fills and spends during play — Health, Mana, Stamina and so on. The pool remembers its current amount, while its bounds come from its [[ResourceType]]: the maximum is usually provided by a backing [[Stat]] (Health's from the Health stat, for example) and moves along with it. Adding to or taking from a pool raises ResourceGain / ResourceLoss events that other effects can react to — a character dies when their Health pool empties down to its minimum.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| type | [[ResourceType]] | True | What kind of pool this is (Health, Mana, …). |
| value | [[Int]] | False | The current amount; setting it is clamped between min and max. |
| max | [[Int]] | True | The most the pool can hold, usually from its backing stat. |
| min | [[Int]] | True | The pool's floor; Health reaching it kills the character. |
| percent | [[Float]] | True | How full the pool is, from 0 to 1. |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Resource#^gain-1525125327\|Gain()]] | [[Void]] | [[Int]] amount | Adds to the pool, up to its maximum. |
| [[Resource#^lose1881468313\|Lose()]] | [[Void]] | [[Int]] amount | Takes from the pool, down to its minimum. |
| [[Resource#^setvalue-1590279867\|SetValue()]] | [[Void]] | [[Int]] value | Sets the pool straight to an amount. |



### Gain ([[Int]] amount) : [[Void]]

^gain-1525125327

Adds to the pool, never past its maximum, and raises a ResourceGain event that other effects can react to.

> [!Example]+ Example
> Restore some of a character's Health when an item is used:
> ```js
> c.Resource('Health').Gain(value);
> ```

> [!Abstract]+ Parameters
> 1. `amount` How much to add. Nothing happens if this is zero or less.

### Lose ([[Int]] amount) : [[Void]]

^lose1881468313

Takes from the pool, never past its minimum, and raises a ResourceLoss event that other effects can react to — losing the last of the Health pool is what kills a character. Note that when dealing damage you usually want [[Character#^takedamage-638525238\|TakeDamage()]] instead, which handles Defense and damage events; Lose() drains the pool directly.

> [!Abstract]+ Parameters
> 1. `amount` How much to take. Nothing happens if this is zero or less.

### SetValue ([[Int]] value) : [[Void]]

^setvalue-1590279867

Sets the pool straight to an amount, clamped between its minimum and maximum. Depending on whether that is more or less than before, it counts as a gain or a loss for events.

> [!Abstract]+ Parameters
> 1. `value` The amount to set the pool to.

