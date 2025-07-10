---
title: CombatManager
draft: false
tags:
 - ScriptObject
---

Can be used in any script through the global alias "Combat".

Example:
```js
// Code for a summon in combat
var c = Asset.SpawnCharacter("bob");
Combat.SpawnUnit(c, u.unit.team, summonLocation);
```


## Variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| isInCombat | [[Bool]] | True |  |
| isPaused | [[Bool]] | True |  |
| currentUnit | [[Unit]] | True | |

## Functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[CombatManager#^getunit\|GetUnit()]] | [[Unit]] | [[GridItem]] position |  |
| [[CombatManager#^getunit2\|GetUnit2()]] | [[Unit]] | [[Int]] x, [[Int]] y | |
| [[CombatManager#^getunits\|GetUnits()]] | [[List]]<[[Unit]]> |  | |
| [[CombatManager#^getdeadunits\|GetDeadUnits()]] | [[List]]<[[Unit]]> |  | |
| [[CombatManager#^getunitsat\|GetUnitsAt()]] | [[List]]<[[Unit]]> | [[GridItem]] position, [[Int]] area | |
| [[CombatManager#^spawnunit\|SpawnUnit()]] | [[Unit]] | [[Character]] c, [[Team]] team, [[GridItem]] position |  |
| [[CombatManager#^removeunit\|RemoveUnit()]] | [[Bool]] | [[GridItem]] position |  |

### GetUnit ([[GridItem]] position) : [[Unit]]

^getunit

Description goes here.

> [!Abstract]+ Parameters
> 1. `position` This is a parameter.

> [!Success]+ Return value
> Returns a [[Unit]].

### GetUnit2 ([[Int]] x, [[Int]] y) : [[Unit]]

^getunit2

Description goes here.

> [!Abstract]+ Parameters
> 1. `x` This is a parameter.
> 2. `y` This is a parameter.

> [!Success]+ Return value
> Returns a [[Unit]].

### GetUnits () : [[List]]<[[Unit]]>

^getunits

Description goes here.

> [!Success]+ Return value
> Returns a [[ETS API/Type/List]]<[[Character]]>.

### GetDeadUnits () : [[List]]<[[Unit]]>

^getdeadunits

Description goes here.

> [!Success]+ Return value
> Returns a [[List]]<[[Unit]]>.

### GetUnitsAt ([[GridItem]] position, [[Int]] area) : [[List]]<[[Unit]]>

^getunitsat

Description goes here.

> [!Abstract]+ Parameters
> 1. `position` This is a parameter.
> 2. `area` This is a parameter.

> [!Success]+ Return value
> Returns a [[List]]<[[Unit]]>.

### SpawnUnit ([[Character]] c, [[Team]] team, [[GridItem]] position) : [[Unit]]

^spawnunit

Description goes here.

> [!Abstract]+ Parameters
> 1. `c` This is a parameter.
> 2. `team` This is a parameter.
> 3. `position` This is a parameter.

> [!Success]+ Return value
> Returns a [[CharacterVisuals]].

### RemoveUnit ([[GridItem]] position) : [[Bool]]

^removeunit

Description goes here.

> [!Abstract]+ Parameters
> 1. `position` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

