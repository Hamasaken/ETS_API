---
title: Ability
draft: false
tags:
 - ScriptType
 - ScriptObject
---
# Ability : [[Any]]

An Ability is an action a [[Character]] can take in combat — an attack, a spell, a heal. It has costs (health and mana), a cooldown, a description shown to the player, and one or more [[CombatEffect]]s that carry out what it actually does. A `CanPerform` script check decides whether it can be used right now.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| description | [[String]] | False | The ability's description text shown to the player. |
| cooldown | [[Int]] | False | Turns that must pass before it can be used again. |
| isReady | [[Int]] | True | True when the ability is off cooldown and usable. |

## Script variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| CanPerform | [[Function]] | False | Your check for whether the character can use the ability now. |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Ability#^finish729994674\|Finish()]] | [[Void]] |  | Signals the ability has finished and starts its cooldown. |

## Script functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |



### Finish () : [[Void]]

^finish729994674

Signals that the ability has finished doing its effect. This starts its cooldown and lets the turn carry on. Call this at the end of an ability's script once its work is done.

