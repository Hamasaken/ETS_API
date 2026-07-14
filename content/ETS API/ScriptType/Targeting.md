---
title: Targeting
draft: false
tags:
 - ScriptType
 - ScriptObject
---
# Targeting : [[Any]]

A Targeting is the set of rules for how an effect picks its targets — how many, at what range, whether it aims at tiles or units, and how large an area of effect it covers. Its script hooks (`CanTarget`, `CanAoe`…) decide which specific tiles and units are allowed. A [[CombatEffect]] uses a Targeting to ask the player to choose, producing a [[TargetingResult]].

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| tileTargeting | [[Bool]] | False | When true, the effect aims at tiles rather than units. |
| amount | [[Int]] | False | How many targets should be chosen. |
| acceptLess | [[Bool]] | False | When true, the effect can proceed with fewer targets. |
| description | [[String]] | False | Text describing the targeting, shown to the player. |
| rangeMin | [[Int]] | False | Closest a target may be (0 for no minimum). |
| rangeMax | [[Int]] | False | Farthest a target may be (0 for no limit). |
| area | [[Int]] | False | Radius of the area of effect around each target (0 for a single tile). |
| overlap | [[Bool]] | False | When true, areas of effect from multiple targets may overlap. |

## Script variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| CanTarget | [[Function]] | False | Your check for whether a unit may be targeted. |
| CanTargetT | [[Function]] | False | Your check for whether a tile may be targeted. |
| CanAoe | [[Function]] | False | Your check for whether a unit is caught in the area of effect. |
| CanAoeT | [[Function]] | False | Your check for whether a tile is caught in the area of effect. |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Script functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |



