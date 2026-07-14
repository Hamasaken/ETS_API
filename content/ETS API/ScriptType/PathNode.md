---
title: PathNode
draft: false
tags:
 - ScriptType
---
# PathNode : [[GridItem]]

A PathNode is one square of the map as [[Pathfinding]] sees it. While a route is worked out, each node remembers how much it costs to step onto, the cheapest total cost to reach it from the unit's starting square, which node the route arrived from, and which neighbouring squares it connects to. Following the chain of `prevNode`s back from a destination traces out the whole path.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| nodeCost | [[Int]] | True | Cost to step onto this square by itself. |
| totalCost | [[Int]] | True | Cheapest total cost to reach this square from the start. |
| fakeCost | [[Int]] | True | Internal working value used while routes are calculated. |
| prevNode | [[PathNode]] | True | The square the cheapest route here came from. |
| connectedNodes | [[List]]<[[PathNode]]> | True | The neighbouring squares this one links to. |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |



