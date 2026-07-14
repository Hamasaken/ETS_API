---
title: Pathfinding
draft: false
tags:
 - ScriptType
---
# Pathfinding : [[Any]]

Pathfinding works out how a unit can move around the [[TileMap]], taking each tile's movement cost into account. From it you can look up a single square as a [[PathNode]], get the full route to a destination, check whether a square is reachable with the unit's movement, and measure the rough movement cost between two points. Diagonal steps cost a little more than straight ones.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Pathfinding#^distancecost1465758219\|DistanceCost()]] | [[Int]] | [[GridItem]] a, [[GridItem]] b | Rough straight-line movement cost between two squares. |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Pathfinding#^getnode1051415311\|GetNode()]] | [[PathNode]] | [[GridItem]] pos | Looks up the pathfinding square at a position. |
| [[Pathfinding#^getpath-792099724\|GetPath()]] | [[List]]<[[PathNode]]> | [[GridItem]] pos | The full route to a destination. |
| [[Pathfinding#^canmoveto-132028670\|CanMoveTo()]] | [[Bool]] | [[GridItem]] pos, \[[[Int]] movementPoints\] | Whether the unit can reach a square. |



### DistanceCost ([[GridItem]] a, [[GridItem]] b) : [[Int]]

^distancecost1465758219

Estimates the movement cost of travelling straight from one square to another, counting diagonal steps as slightly more expensive than straight ones. It ignores walls and terrain, so it's a quick as-the-crow-flies measure rather than the cost of a real route.

> [!Abstract]+ Parameters
> 1. `a` The square to measure from.
> 2. `b` The square to measure to.

> [!Success]+ Return value
> Returns the estimated straight-line movement cost between the two squares.

### GetNode ([[GridItem]] pos) : [[PathNode]]

^getnode1051415311

Looks up the pathfinding square at a grid position, giving you its costs and route information as a [[PathNode]].

> [!Abstract]+ Parameters
> 1. `pos` The grid position to look up.

> [!Success]+ Return value
> Returns the pathfinding square at that position.

### GetPath ([[GridItem]] pos) : [[List]]<[[PathNode]]>

^getpath-792099724

Gives the route the unit would take to reach a position, as an ordered list of squares running from its current square through to the destination.

> [!Abstract]+ Parameters
> 1. `pos` Where the unit is heading.

> [!Success]+ Return value
> Returns the ordered list of squares making up the route.

### CanMoveTo ([[GridItem]] pos, \[[[Int]] movementPoints\]) : [[Bool]]

^canmoveto-132028670

Checks whether the unit can actually reach a square. By default it measures against the unit's remaining movement this turn; give a movement budget to test against a different amount instead.

> [!Abstract]+ Parameters
> 1. `pos` The square to test.
> 2. `movementPoints` A movement budget to test against. Leave out to use the unit's remaining movement.

> [!Success]+ Return value
> Returns true if the square can be reached within the movement budget.

