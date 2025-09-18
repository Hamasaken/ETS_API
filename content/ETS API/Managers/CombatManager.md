---
title: CombatManager
draft: false
tags:
 - ScriptObject
---

The combat manager is responsible for keeping track of units and the map itself during fight scenes.

Can be used in any script through the global alias "Combat".

Example:
```js
// Code for a summon in combat.
var c = Asset.SpawnCharacter("bob");
Combat.SpawnUnit(c, u.unit.team, summonLocation);
```

> [!Warning]
> Most of these functions can only be used safely while a fight is currently ongoing. You can check for this by reading the public variable "isInCombat."

Example:
```js
if (Combat.isInCombat) {
	// Run combat functions safely here.
}
```


## Variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| isInCombat | [[Bool]] | True |  |
| isPaused | [[Bool]] | True |  |
| currentUnit | [[Unit]] | True |  |

## Functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[CombatManager#^getunit\|GetUnit()]] | [[Unit]] | [[GridItem]] position |  |
| [[CombatManager#^getunit2\|GetUnit2()]] | [[Unit]] | [[Int]] x, [[Int]] y |  |
| [[CombatManager#^getunits\|GetUnits()]] | [[List]]<[[Unit]]> |  |  |
| [[CombatManager#^getdeadunits\|GetDeadUnits()]] | [[List]]<[[Unit]]> |  |  |
| [[CombatManager#^getunitsat\|GetUnitsAt()]] | [[List]]<[[Unit]]> | [[GridItem]] position, [[Int]] area |  |
| [[CombatManager#^spawnunit\|SpawnUnit()]] | [[Unit]] | [[Character]] c, [[Team]] team, [[GridItem]] position |  |
| [[CombatManager#^removeunit\|RemoveUnit()]] | [[Bool]] | [[GridItem]] position |  |

### GetUnit ([[GridItem]] position) : [[Unit]]

^getunit

Fetches the [[Unit]] at the specified position. Returns null if the position in unoccupied.

> [!Abstract]+ Parameters
> 1. `position` The position of the requested unit.

> [!Success]+ Return value
> Returns the [[Unit]] at the position, otherwise [[Null]].

### GetUnit2 ([[Int]] x, [[Int]] y) : [[Unit]]

^getunit2

Fetches the [[Unit]] at the specified position. Returns null if the position in unoccupied.

> [!Abstract]+ Parameters
> 1. `x` The x value of the requested unit.
> 2. `y` The y value of the requested unit.

> [!Success]+ Return value
> Returns the [[Unit]] at the position, otherwise [[Null]].

### GetUnits () : [[List]]<[[Unit]]>

^getunits

Fetches a list of every participating unit that is ***still alive***. Use [[CombatManager#^getdeadunits\|GetDeadUnits()]] to retrieve the dead units instead.

> [!Success]+ Return value
> Returns a [[List]]<[[Character]]>.

### GetDeadUnits () : [[List]]<[[Unit]]>

^getdeadunits

Fetches a list of every participating unit that is dead.

> [!Success]+ Return value
> Returns a [[List]]<[[Unit]]>.

### GetUnitsAt ([[GridItem]] position, [[Int]] area) : [[List]]<[[Unit]]>

^getunitsat

Fetches a list of every unit within an area centered on the specified position.

> [!Abstract]+ Parameters
> 1. `position` The position of the center tile.
> 2. `area` The radius of the circular area in mapunits. 10 = one tile straight, 14 = one tile diagonally.

> [!Success]+ Return value
> Returns a [[List]]<[[Unit]]>.

### SpawnUnit ([[Character]] c, [[Team]] team, [[GridItem]] position) : [[Unit]]

^spawnunit

Spawns a new unit and places it onto the battlefield. The unit will represent the character "c" and will belong to the specified team.

> [!Abstract]+ Parameters
> 1. `c` The character to place onto the battlefield.
> 2. `team` What team the character will join. See [[Team]] for possible values.
> 3. `position` The position the unit will be placed at. Will not work if the position is occupied.

> [!Success]+ Return value
> Returns the newly created [[Unit]] instance.

### RemoveUnit ([[GridItem]] position) : [[Bool]]

^removeunit

Removes the unit at the specified position.

> [!Abstract]+ Parameters
> 1. `position` This is a parameter.

> [!Success]+ Return value
> Returns [[Bool|true]] if a unit was found at the position and successfully removed. Otherwise, returns [[Bool|false]].

