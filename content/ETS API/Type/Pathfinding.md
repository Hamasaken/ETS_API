---
title: Pathfinding
draft: false
tags:
 - ScriptObject
---

Description goes here.

## Variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Pathfinding#^getnode\|GetNode()]] | [[PathNode]] | [[GridItem]] pos |  |
| [[Pathfinding#^getpath\|GetPath()]] | [[List]]<[[PathNode]]> | [[GridItem]] pos |  |
| [[Pathfinding#^canmoveto\|CanMoveTo()]] | [[Bool]] | [[GridItem]] pos, [[Int]] movementPoints |  |
| [[Pathfinding#^distancecost\|DistanceCost()]] | [[Int]] | [[GridItem]] a, [[GridItem]] b |  |

### GetNode ([[GridItem]] pos) : [[PathNode]]

^getnode

Description goes here.

> [!Abstract]+ Parameters
> 1. `pos` This is a parameter.

> [!Success]+ Return value
> Returns a [[PathNode]].

### GetPath ([[GridItem]] pos) : [[List]]<[[PathNode]]>

^getpath

Description goes here.

> [!Abstract]+ Parameters
> 1. `pos` This is a parameter.

> [!Success]+ Return value
> Returns a [[List]]<[[PathNode]]>.

### CanMoveTo ([[GridItem]] pos, [[Int]] movementPoints) : [[Bool]]

^canmoveto

Description goes here.

> [!Abstract]+ Parameters
> 1. `pos` This is a parameter.
> 2. `movementPoints` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### DistanceCost ([[GridItem]] a, [[GridItem]] b) : [[Int]]

^distancecost

Description goes here.

> [!Abstract]+ Parameters
> 1. `a` This is a parameter.
> 2. `b` This is a parameter.

> [!Success]+ Return value
> Returns a [[Int]].

