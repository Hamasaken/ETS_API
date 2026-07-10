---
title: Combat
draft: false
tags:
 - Scope
---
# Combat

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


## Script variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| isInCombat | [[Bool]] | True |  |
| isPaused | [[Bool]] | True |  |
| currentUnit | [[Unit]] | True |  |


## Script functions
| Name                                 | Return type             | Parameters                            | Note |
| ------------------------------------ | ----------------------- | ------------------------------------- | ---- |
| [[Combat#^getunit928097881\|GetUnit()]] | [[Unit]] | [[GridItem]] position |  |
| [[Combat#^getunit-1294198661\|GetUnit()]] | [[Unit]] | [[Int]] x, [[Int]] y |  |
| [[Combat#^getunits-95537766\|GetUnits()]] | [[List]]<[[Unit]]> |  |  |
| [[Combat#^getdeadunits1569739442\|GetDeadUnits()]] | [[List]]<[[Unit]]> |  |  |
| [[Combat#^getunitsat-1156936270\|GetUnitsAt()]] | [[List]]<[[Unit]]> | [[GridItem]] position, [[Int]] area |  |
| [[Combat#^spawnunit2032907621\|SpawnUnit()]] | [[Unit]] | [[Character]] c, [[TeamType]] team, [[GridItem]] position |  |
| [[Combat#^removeunit1369825921\|RemoveUnit()]] | [[Bool]] | [[GridItem]] position |  |
| [[Combat#^moveunit1533025612\|MoveUnit()]] | [[Bool]] | [[Unit]] unit, [[Movement]] movement, \[[[Bool]] forced\] | |


### GetUnit ([[GridItem]] position) : [[Unit]]

^getunit928097881

This is a function.

> [!Abstract]+ Parameters
> 1. `position` This is a parameter.

> [!Success]+ Return value
> Returns a [[Unit]].

### GetUnit ([[Int]] x, [[Int]] y) : [[Unit]]

^getunit-1294198661

This is a function.

> [!Abstract]+ Parameters
> 1. `x` This is a parameter.
> 2. `y` This is a parameter.

> [!Success]+ Return value
> Returns a [[Unit]].

### GetUnits () : [[List]]<[[Unit]]>

^getunits-95537766

This is a function.

> [!Success]+ Return value
> Returns a [[List]]<[[Character]]>.

### GetDeadUnits () : [[List]]<[[Unit]]>

^getdeadunits1569739442

This is a function.

> [!Success]+ Return value
> Returns a [[List]]<[[Unit]]>.

### GetUnitsAt ([[GridItem]] position, [[Int]] area) : [[List]]<[[Unit]]>

^getunitsat-1156936270

This is a function.

> [!Abstract]+ Parameters
> 1. `position` This is a parameter.
> 2. `area` This is a parameter.

> [!Success]+ Return value
> Returns a [[List]]<[[Unit]]>.

### SpawnUnit ([[Character]] c, [[TeamType]] team, [[GridItem]] position) : [[Unit]]

^spawnunit2032907621

This is a function.

> [!Abstract]+ Parameters
> 1. `c` This is a parameter.
> 2. `team` This is a parameter.
> 3. `position` This is a parameter.

> [!Success]+ Return value
> Returns a [[UnitVisuals]].

### RemoveUnit ([[GridItem]] position) : [[Bool]]

^removeunit1369825921

This is a function.

> [!Abstract]+ Parameters
> 1. `position` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### MoveUnit ([[Unit]] unit, [[Movement]] movement, \[[[Bool]] forced\]) : [[Bool]]

^moveunit1533025612

This is a function.

> [!Abstract]+ Parameters
> 1. `unit` This is a parameter.
> 2. `movement` This is a parameter.
> 3. `forced` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

