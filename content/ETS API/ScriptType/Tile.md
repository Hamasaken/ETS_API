---
title: Tile
draft: false
tags:
 - ScriptType
---
# Tile : [[GridItem]]

A Tile is a single square of the combat map at a grid position. Its [[TileType]] decides what the square is — floor, water, wall, and so on — which in turn sets how costly, or impossible, it is to move across. A Tile takes its position on the map from [[GridItem]].

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| type | [[TileType]] | True | What kind of square this is (floor, wall, water…). |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Tile#^getmaxcost933763044\|GetMaxCost()]] | [[Int]] |  | Highest movement cost this kind of tile can charge. |
| [[Tile#^getcost1974256603\|GetCost()]] | [[Int]] | [[Unit]] unit | Movement cost for a specific unit to enter. |
| [[Tile#^getcost1974247210\|GetCost()]] | [[Int]] | [[Character]] character | Movement cost for a specific character to enter. |



### GetMaxCost () : [[Int]]

^getmaxcost933763044

Gives the highest movement cost this kind of tile can charge anyone to cross. Handy as a worst-case figure when you don't have a particular unit in mind.

> [!Success]+ Return value
> Returns the tile's highest possible movement cost.

### GetCost ([[Unit]] unit) : [[Int]]

^getcost1974256603

Works out how much movement it costs this particular unit to step onto the tile. The cost depends on the unit's traits and flags, so a flyer or swimmer may cross terrain cheaply that slows others down. Impassable tiles such as walls return a very large cost, effectively blocking the way.

> [!Abstract]+ Parameters
> 1. `unit` The unit that would move onto the tile.

> [!Success]+ Return value
> Returns the movement cost for this unit, or a very large number if the tile is impassable to it.

### GetCost ([[Character]] character) : [[Int]]

^getcost1974247210

The same as the unit version, but for a [[Character]] — useful before the character is placed on the grid as a unit. The cost depends on the character's traits and flags, and impassable tiles return a very large cost.

> [!Abstract]+ Parameters
> 1. `character` The character that would move onto the tile.

> [!Success]+ Return value
> Returns the movement cost for this character, or a very large number if the tile is impassable to them.

