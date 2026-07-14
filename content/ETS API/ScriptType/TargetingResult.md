---
title: TargetingResult
draft: false
tags:
 - ScriptType
---
# TargetingResult : [[Any]]

A TargetingResult is the full outcome of a targeting step — the list of [[Target]]s that were chosen. It also offers quick ways to pull out just the tiles, units, or characters involved. A [[CombatEffect]] receives one of these after asking the player to pick targets.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| targets | [[List]]<[[Target]]> | True | All the targets that were chosen. |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[TargetingResult#^gettiles325254240\|GetTiles()]] | [[List]]<[[Tile]]> |  | Just the tiles from all chosen targets. |
| [[TargetingResult#^getunits-95537766\|GetUnits()]] | [[List]]<[[Unit]]> |  | Just the units from all chosen targets. |
| [[TargetingResult#^getcharacters-291915489\|GetCharacters()]] | [[List]]<[[Character]]> |  | The characters of all targeted units. |



### GetTiles () : [[List]]<[[Tile]]>

^gettiles325254240

Gathers the tiles from every chosen target into a single list, ignoring any targets that were units rather than tiles.

> [!Success]+ Return value
> Returns the list of every targeted tile.

### GetUnits () : [[List]]<[[Unit]]>

^getunits-95537766

Gathers the units from every chosen target into a single list, ignoring any targets that were tiles rather than units.

> [!Success]+ Return value
> Returns the list of every targeted unit.

### GetCharacters () : [[List]]<[[Character]]>

^getcharacters-291915489

Gathers the characters of every targeted unit into a single list — a shortcut when you want to act on the characters rather than their grid pieces.

> [!Success]+ Return value
> Returns the list of every targeted character.

