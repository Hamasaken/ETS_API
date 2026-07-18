---
title: Type
draft: false
tags:
  - ScriptType
  - ClassEnum
aliases:
  - ScriptTypes
---

# ScriptType : [[ClassEnum]]


ETScript is a softly typed scripting language. Behind the scenes, all of the data is handled as C# objects and classes, wrapped into a selection of "ETS ScriptTypes".

> [!Note]
> Even though not all common C# types have an ETS counterpart, the scripting language is still able to access C# objects and pass them around as parameters. However, accessing member fields and methods on those objects is not possible from ETS.


## Enum values
| Id   | Name                  | BaseType              | Description |
| ---- | --------------------- | --------------------- | ----------- |
| 0 | [[Any]] |   |  |
| 1 | [[Null]] |   |  |
| 2 | [[Void]] |   |  |
| 10 | [[String]] | [[Any]]  |  |
| 11 | [[Int]] | [[Any]]  |  |
| 12 | [[Float]] | [[Any]]  |  |
| 13 | [[Bool]] | [[Any]]  |  |
| 20 | [[List]] | [[Any]]  |  |
| 21 | [[Dictionary]] | [[Any]]  |  |
| 30 | [[Scope]] | [[Any]]  |  |
| 31 | [[Instruction]] | [[Any]]  |  |
| 32 | [[Expression]] | [[Any]]  |  |
| 40 | [[FunctionBase]] | [[Any]]  |  |
| 41 | [[Function]] | [[FunctionBase]]  |  |
| 42 | [[Lambda]] | [[FunctionBase]]  |  |
| 50 | [[EventListener]] | [[Any]]  |  |
| 51 | [[EventData]] | [[Any]]  |  |
| 52 | [[EventAware]] | [[Any]]  |  |
| 100 | [[Stat]] | [[Any]]  |  |
| 101 | [[Flag]] | [[Any]]  |  |
| 102 | [[Resource]] | [[Any]]  |  |
| 200 | [[BaseAsset]] | [[Any]]  |  |
| 210 | [[Character]] | [[BaseAsset]]  |  |
| 211 | [[Item]] | [[EventAware]]  |  |
| 212 | [[Status]] | [[EventAware]], [[BaseAsset]]  |  |
| 213 | [[Trait]] | [[EventAware]]  |  |
| 250 | [[Ability]] | [[Any]]  |  |
| 251 | [[CombatEffect]] | [[Any]]  |  |
| 252 | [[Attack]] | [[Any]]  |  |
| 253 | [[Damage]] | [[Any]]  |  |
| 254 | [[StatScaling]] | [[Any]]  |  |
| 300 | [[ClassEnum]] | [[Any]]  |  |
| 310 | [[ScriptType]] | [[ClassEnum]]  |  |
| 311 | [[TraitGroup]] | [[ClassEnum]]  |  |
| 312 | [[TraitType]] | [[ClassEnum]]  |  |
| 313 | [[StatType]] | [[ClassEnum]]  |  |
| 314 | [[DamageType]] | [[ClassEnum]]  |  |
| 315 | [[EventType]] | [[ClassEnum]]  |  |
| 316 | [[AttackType]] | [[ClassEnum]]  |  |
| 317 | [[FlagType]] | [[ClassEnum]]  |  |
| 318 | [[TileType]] | [[ClassEnum]]  |  |
| 319 | [[TeamType]] | [[ClassEnum]]  |  |
| 320 | [[ResourceType]] | [[ClassEnum]]  |  |
| 400 | [[Verse]] | [[Any]]  |  |
| 401 | [[Line]] | [[Any]]  |  |
| 500 | [[TileMap]] | [[Any]]  |  |
| 501 | [[Pathfinding]] | [[Any]]  |  |
| 510 | [[GridItem]] | [[Any]]  |  |
| 511 | [[PathNode]] | [[GridItem]]  |  |
| 512 | [[Tile]] | [[GridItem]]  |  |
| 513 | [[Unit]] | [[GridItem]]  |  |
| 520 | [[Targeting]] | [[Any]]  |  |
| 521 | [[Target]] | [[GridItem]]  |  |
| 522 | [[TargetingResult]] | [[Any]]  |  |
| 530 | [[Movement]] | [[Any]]  |  |
| 1000 | [[Vector2D]] | [[Any]]  |  |
| 1001 | [[Vector3D]] | [[Any]]  |  |
| 1100 | [[AnimationListener]] | [[Any]]  |  |
| 1101 | [[CharacterVisuals]] | [[AnimationListener]]  |  |
| 1102 | [[UnitVisuals]] | [[CharacterVisuals]]  |  |
| 1110 | [[Projectile]] | [[Any]]  |  |


## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

