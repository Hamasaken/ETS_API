---
title: CombatManager
draft: false
tags:
 - ScriptObject
---

Description goes here.

## Variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| isInCombat | [[Bool]] | True |  |

## Functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[CombatManager#^getunits\|GetUnits()]] | [[List]]<[[Character]]> |  |  |
| [[CombatManager#^spawnunit\|SpawnUnit()]] | [[CharacterVisuals]] | [[Character]] c, [[GridItem]] pos |  |
| [[CombatManager#^spawnunit2\|SpawnUnit2()]] | [[CharacterVisuals]] | [[Character]] c, [[Int]] x, [[Int]] y | |
| [[CombatManager#^removeunit\|RemoveUnit()]] | [[Bool]] | [[Character]] c |  |

### GetUnits () : [[List]]<[[Character]]>

^getunits

Description goes here.

> [!Success]+ Return value
> Returns a [[List]]<[[Character]]>.

### SpawnUnit ([[Character]] c, [[GridItem]] pos) : [[CharacterVisuals]]

^spawnunit

Description goes here.

> [!Abstract]+ Parameters
> 1. `c` This is a parameter.
> 2. `pos` This is a parameter.

> [!Success]+ Return value
> Returns a [[CharacterVisuals]].

### SpawnUnit2 ([[Character]] c, [[Int]] x, [[Int]] y) : [[CharacterVisuals]]

^spawnunit2

Description goes here.

> [!Abstract]+ Parameters
> 1. `c` This is a parameter.
> 2. `x` This is a parameter.
> 3. `y` This is a parameter.

> [!Success]+ Return value
> Returns a [[CharacterVisuals]].

### RemoveUnit ([[Character]] c) : [[Bool]]

^removeunit

Description goes here.

> [!Abstract]+ Parameters
> 1. `c` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

