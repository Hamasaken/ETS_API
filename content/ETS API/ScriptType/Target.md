---
title: Target
draft: false
tags:
 - ScriptType
---
# Target : [[GridItem]]

A Target is one thing an ability or effect has been aimed at — a single [[Tile]] or [[Unit]] on the grid, along with the area around it that the effect covers. From it you can read the exact tile or unit that was chosen, and the lists of tiles, units, and characters caught in its area of effect.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| tile | [[Tile]] | True | The exact tile targeted, if a tile was chosen. |
| unit | [[Unit]] | True | The exact unit targeted, if a unit was chosen. |
| areaTiles | [[List]]<[[Tile]]> | True | Every tile covered by the area of effect. |
| areaUnits | [[List]]<[[Unit]]> | True | Every unit standing in the area of effect. |
| areaCharacters | [[List]]<[[Character]]> | True | The characters of every unit in the area of effect. |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |



