---
title: Movement
draft: false
tags:
 - ScriptType
---
# Movement : [[Any]]

A Movement describes a single move a unit makes: the route it takes across the grid, where it starts and ends, how much it costs, and how it should look while moving (which animation to play and how long it takes). Effects and abilities build a Movement to slide a unit from one square to another.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| path | [[List]]<[[PathNode]]> | True | The ordered squares the unit travels through. |
| start | [[GridItem]] | True | The square the move begins on. |
| end | [[GridItem]] | True | The square the move finishes on. |
| totalCost | [[Int]] | True | Total movement cost of the whole move. |
| hasSteps | [[Bool]] | True | True when the move follows a full step-by-step route. |
| time | [[Float]] | False | How long the movement takes, in seconds. |
| animation | [[String]] | False | The animation to play while moving. |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Movement#^setpath-142726015\|SetPath()]] | [[Void]] | [[List]]<[[PathNode]]> path | Follow a ready-made route of squares. |
| [[Movement#^setpath-145803660\|SetPath()]] | [[Void]] | [[GridItem]] start, [[GridItem]] end | Move directly from one square to another. |



### SetPath ([[List]]<[[PathNode]]> path) : [[Void]]

^setpath-142726015

Sets the move to follow a ready-made route — a list of squares — and works out its start, end and total cost from that route.

> [!Abstract]+ Parameters
> 1. `path` The ordered squares the unit should travel through.

### SetPath ([[GridItem]] start, [[GridItem]] end) : [[Void]]

^setpath-145803660

Sets the move as a direct jump from one square straight to another, without a step-by-step route in between.

> [!Abstract]+ Parameters
> 1. `start` The square the move begins on.
> 2. `end` The square the move finishes on.

