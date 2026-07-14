---
title: Unit
draft: false
tags:
 - ScriptType
---
# Unit : [[GridItem]]

A Unit is a [[Character]] as it appears on the combat grid — a single combatant with a grid position, a team, and a pool of actions and movement for the current turn. Most combat scripting (ability targeting, area-of-effect rules, and effects) operates on Units. It inherits everything from [[GridItem]], so a Unit also has a position on the map.

## Static variables
| Name | Type       | Readonly | Note                     |
| ---- | ---------- | -------- | ------------------------ |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| uid | [[String]] | True | The unit's unique id (the same id as its character). |
| visuals | [[UnitVisuals]] | True | The unit's on-screen visual representation. |
| c | [[Character]] | True | Shorthand alias for `character`. |
| character | [[Character]] | True | The character this unit represents in combat. |
| team | [[TeamType]] | False | Which side the unit fights for; can be changed at runtime. |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Unit#^isally1240438894\|IsAlly()]] | [[Bool]] | [[Unit]] unit | True when the other unit is friendly. |
| [[Unit#^isenemy-960203908\|IsEnemy()]] | [[Bool]] | [[Unit]] unit | True when the other unit is hostile. |



### IsAlly ([[Unit]] unit) : [[Bool]]

^isally1240438894

Checks whether another unit is friendly to this one. Units on the same team are allies. A neutral unit is treated as an ally to everyone, so this also returns true when the other unit is neutral.

> [!Example]+ Example
> Only let a healing ability target friendly units:
> ```js
> "canTarget": "u.IsAlly(t)"
> ```

> [!Abstract]+ Parameters
> 1. `unit` The other unit to check against this one.

> [!Success]+ Return value
> Returns true when both units are on the same team, or when `unit` is neutral.

### IsEnemy ([[Unit]] unit) : [[Bool]]

^isenemy-960203908

Checks whether another unit is hostile to this one. Units on opposing teams are enemies. A neutral unit is treated as an enemy to everyone, so this also returns true when the other unit is neutral.

> [!Example]+ Example
> Only let an attack target hostile units:
> ```js
> "canTarget": "u.IsEnemy(t)"
> ```

> [!Abstract]+ Parameters
> 1. `unit` The other unit to check against this one.

> [!Success]+ Return value
> Returns true when the units are on different teams, or when `unit` is neutral.

