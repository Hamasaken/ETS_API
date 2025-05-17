---
title: Type
draft: false
tags:
 - ClassEnum
aliases:
 - Types
 - VariableType
 - VariableTypes
---

ETScript is a softly typed scripting language. Behind the scenes, all of the data is handled as C# objects and classes, wrapped into a selection of "ETS types".

> [!Note]
> Even though not all common C# types have an ETS counterpart, the scripting language is still able to access the C# objects and pass them around. However, accessing member fields and methods on those objects is not possible from ETS.

## Values
| id  | name                 | description                                                            |
| --- | -------------------- | ---------------------------------------------------------------------- |
| 0 | [[Any]]  | This is the fallback type for C# objects that are not valid ETS types. |
| 1 | [[Null]]  | The representation of an empty variable. |
| 2 | [[Void]]  | The lack of a return type for a [[Function]]. |
| 10 | [[String]]  | A string of characters, ex: `"Mikael"` |
| 11 | [[Int]]  | An integer number. |
| 12 | [[Float]]  | A floating point number. |
| 13 | [[Bool]]  | A boolean value. Can only be `true` or `false`. |
| 20 | [[List]]  | A list of a certain type of variables. |
| 21 | [[Dictionary]]  | A dictionary with a certain type of key-value pairs. |
| 30 | [[Scope]]  |  |
| 31 | [[Instruction]]  |  |
| 32 | [[Expression]]  |  |
| 33 | [[Namespace]]  |  |
| 40 | [[Function]]  |  |
| 41 | [[EventListener]]  |  |
| 50 | [[EEvent]]  |  |
| 100 | [[Stat]]  |  |
| 101 | [[Trait]]  |  |
| 102 | [[Flag]]  |  |
| 103 | [[Team]]  |  |
| 200 | [[Character]]  | This is just a guy. |
| 201 | [[Attack]]  |  |
| 202 | [[Damage]]  |  |
| 203 | [[Targeting]]  |  |
| 204 | [[StatScaling]]  |  |
| 210 | [[StatusEffect]]  |  |
| 220 | [[Item]]  |  |
| 300 | [[Type]]  |  |
| 301 | [[TraitType]]  |  |
| 302 | [[StatType]]  |  |
| 303 | [[StatAction]]  |  |
| 304 | [[DamageType]]  |  |
| 305 | [[EventType]]  |  |
| 306 | [[AttackType]]  |  |
| 307 | [[FlagType]]  |  |
| 308 | [[TileType]]  |  |
| 400 | [[Vector2D]]  |  |
| 401 | [[Vector3D]]  |  |
| 402 | [[GridItem]]  |  |
| 403 | [[PathNode]]  |  |
| 410 | [[Tile]]  |  |
| 500 | [[CharacterVisuals]]  |  |
| 501 | [[Projectile]]  |  |
| 502 | [[AnimationListener]]  |  |
