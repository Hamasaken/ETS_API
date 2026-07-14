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
| isInCombat | [[Bool]] | True | True while a fight is currently taking place. |
| isPaused | [[Bool]] | True | True when combat is paused. |
| currentUnit | [[Unit]] | True | The unit whose turn it currently is. |


## Script functions
| Name                                 | Return type             | Parameters                            | Note |
| ------------------------------------ | ----------------------- | ------------------------------------- | ---- |
| [[Combat#^getunit928097881\|GetUnit()]] | [[Unit]] | [[GridItem]] position | The unit standing on a position. |
| [[Combat#^getunit-1294198661\|GetUnit()]] | [[Unit]] | [[Int]] x, [[Int]] y | The unit at a column and row. |
| [[Combat#^getunits-95537766\|GetUnits()]] | [[List]]<[[Unit]]> |  | Every living unit in the fight. |
| [[Combat#^getdeadunits1569739442\|GetDeadUnits()]] | [[List]]<[[Unit]]> |  | Every defeated unit in the fight. |
| [[Combat#^getunitsat-1156936270\|GetUnitsAt()]] | [[List]]<[[Unit]]> | [[GridItem]] position, [[Int]] area | Every unit within a radius of a position. |
| [[Combat#^spawnunit2032907621\|SpawnUnit()]] | [[Unit]] | [[Character]] c, [[TeamType]] team, [[GridItem]] position | Places a character into the fight. |
| [[Combat#^removeunit1369825921\|RemoveUnit()]] | [[Bool]] | [[GridItem]] position | Removes the unit at a position. |
| [[Combat#^moveunit1533025612\|MoveUnit()]] | [[Bool]] | [[Unit]] unit, [[Movement]] movement, \[[[Bool]] forced\] | Moves a unit along a path. |


### GetUnit ([[GridItem]] position) : [[Unit]]

^getunit928097881

Finds the unit standing on a grid position, or gives nothing back if that tile is empty.

> [!Abstract]+ Parameters
> 1. `position` The grid position to check.

> [!Success]+ Return value
> Returns the unit on that tile, or nothing if it's empty.

### GetUnit ([[Int]] x, [[Int]] y) : [[Unit]]

^getunit-1294198661

Finds the unit at the given column and row, or gives nothing back if that tile is empty. The same as the other [[Combat#^getunit928097881\|GetUnit()]] but with the position given as two numbers.

> [!Abstract]+ Parameters
> 1. `x` The column, counted from 0.
> 2. `y` The row, counted from 0.

> [!Success]+ Return value
> Returns the unit on that tile, or nothing if it's empty.

### GetUnits () : [[List]]<[[Unit]]>

^getunits-95537766

Gives every living unit currently taking part in the fight.

> [!Success]+ Return value
> Returns the list of all living units in the fight.

### GetDeadUnits () : [[List]]<[[Unit]]>

^getdeadunits1569739442

Gives every unit that has been defeated so far in the fight — useful for effects that raise or target the fallen.

> [!Success]+ Return value
> Returns the list of all defeated units in the fight.

### GetUnitsAt ([[GridItem]] position, [[Int]] area) : [[List]]<[[Unit]]>

^getunitsat-1156936270

Gives every unit within a given radius of a position — the tool for finding who is caught in an area-of-effect blast.

> [!Example]+ Example
> Find all units in the blast area around a bomb:
> ```js
> var hits = Combat.GetUnitsAt(c.unit, area);
> ```

> [!Abstract]+ Parameters
> 1. `position` The centre of the area to search.
> 2. `area` How far out from the centre to look.

> [!Success]+ Return value
> Returns the list of units within that radius.

### SpawnUnit ([[Character]] c, [[TeamType]] team, [[GridItem]] position) : [[Unit]]

^spawnunit2032907621

Places a [[Character]] into the current fight as a new unit, on the given team and at the given position. This is how summons and reinforcements appear mid-battle.

> [!Example]+ Example
> Summon a character onto the caster's team:
> ```js
> var c = Asset.SpawnCharacter("bob");
> Combat.SpawnUnit(c, u.unit.team, summonLocation);
> ```

> [!Abstract]+ Parameters
> 1. `c` The character to bring into the fight.
> 2. `team` Which side the new unit fights for.
> 3. `position` Where on the grid to place it.

> [!Success]+ Return value
> Returns the newly placed unit.

### RemoveUnit ([[GridItem]] position) : [[Bool]]

^removeunit1369825921

Takes the unit at a grid position out of the fight entirely.

> [!Abstract]+ Parameters
> 1. `position` The grid position of the unit to remove.

> [!Success]+ Return value
> Returns true if there was a unit there to remove.

### MoveUnit ([[Unit]] unit, [[Movement]] movement, \[[[Bool]] forced\]) : [[Bool]]

^moveunit1533025612

Moves a unit across the grid following a prepared [[Movement]]. Turn on `forced` to move the unit even when it normally couldn't act — for example a knockback or a pull.

> [!Abstract]+ Parameters
> 1. `unit` The unit to move.
> 2. `movement` The move to carry out (its path, start and end).
> 3. `forced` True to move the unit even when it can't act normally. Leave out for a normal move.

> [!Success]+ Return value
> Returns true if the unit was moved.

