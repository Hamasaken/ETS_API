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
| 0 | [[Any]] |   | A value of any type; the common ancestor of all types. |
| 1 | [[Null]] |   | "No value" — an empty slot where a value could be. |
| 2 | [[Void]] |   | Marks functions that return nothing. |
| 10 | [[String]] | [[Any]]  | A piece of text, such as a name or a message. |
| 11 | [[Int]] | [[Any]]  | A whole number, like 0, 5 or -3. |
| 12 | [[Float]] | [[Any]]  | A number with a decimal part, like 0.5 or 1.25. |
| 13 | [[Bool]] | [[Any]]  | A true/false value; what conditions evaluate to. |
| 20 | [[List]] | [[Any]]  | An ordered collection of values. |
| 21 | [[Dictionary]] | [[Any]]  | Stores values by key, for lookup by name. |
| 30 | [[Scope]] | [[Any]]  | The variables and functions available where a script runs. |
| 31 | [[Instruction]] | [[Any]]  | A single step of a running script (internal). |
| 32 | [[Expression]] | [[Any]]  | A piece of script that works out a value (internal). |
| 40 | [[FunctionBase]] | [[Any]]  | Shared base of everything callable. |
| 41 | [[Function]] | [[FunctionBase]]  | A named, reusable piece of script logic. |
| 42 | [[Lambda]] | [[FunctionBase]]  | A small unnamed function written inline where it's used. |
| 50 | [[EventListener]] | [[Any]]  | Watches for a game event and reacts when it happens. |
| 51 | [[EventData]] | [[Any]]  | The details of one game event as it happens. |
| 52 | [[EventAware]] | [[Any]]  | Base for things that can register event listeners. |
| 100 | [[Stat]] | [[Any]]  | One numeric attribute of a character, such as Strength. |
| 101 | [[Flag]] | [[Any]]  | An on/off switch stored on a character, such as Alive. |
| 102 | [[Resource]] | [[Any]]  | A pool a character fills and spends, such as Health or Mana. |
| 200 | [[BaseAsset]] | [[Any]]  | Shared foundation of the game's loadable content. |
| 210 | [[Character]] | [[BaseAsset]]  | A person in the game — party member, enemy or NPC. |
| 211 | [[Item]] | [[EventAware]]  | Something a character can carry, use, consume or equip. |
| 212 | [[Status]] | [[EventAware]], [[BaseAsset]]  | A temporary effect on a character, like a poison or a buff. |
| 213 | [[Trait]] | [[EventAware]]  | One characteristic of a character or item, like Undead. |
| 250 | [[Ability]] | [[Any]]  | An action a character can take in combat. |
| 251 | [[CombatEffect]] | [[Any]]  | One step of what an ability or item does in battle. |
| 252 | [[Attack]] | [[Any]]  | How a strike is delivered, and its base accuracy. |
| 253 | [[Damage]] | [[Any]]  | A hit dealt to a character: amount, type and penetration. |
| 254 | [[StatScaling]] | [[Any]]  | How an effect grows with one of the user's stats. |
| 300 | [[ClassEnum]] | [[Any]]  | A named set of options, extendable through asset files. |
| 310 | [[ScriptType]] | [[ClassEnum]]  | This enum — the value types of the scripting language. |
| 311 | [[TraitGroup]] | [[ClassEnum]]  | The groups traits are organised into, like Race or Job. |
| 312 | [[TraitType]] | [[ClassEnum]]  | The individual traits characters and items can have. |
| 313 | [[StatType]] | [[ClassEnum]]  | The kinds of statistic a character can have. |
| 314 | [[DamageType]] | [[ClassEnum]]  | The elemental types damage can have. |
| 315 | [[EventType]] | [[ClassEnum]]  | The kinds of game event listeners can watch for. |
| 316 | [[AttackType]] | [[ClassEnum]]  | The ways a strike can be delivered, such as Melee or Ranged. |
| 317 | [[FlagType]] | [[ClassEnum]]  | The kinds of on/off flag a character can have. |
| 318 | [[TileType]] | [[ClassEnum]]  | The kinds of tile a map is built from; sets movement cost. |
| 319 | [[TeamType]] | [[ClassEnum]]  | The team a unit fights for; decides allies and enemies. |
| 320 | [[ResourceType]] | [[ClassEnum]]  | The kinds of resource pool and how each behaves. |
| 400 | [[Verse]] | [[Any]]  | A scripted scene of story or conversation. |
| 401 | [[Line]] | [[Any]]  | A single step of a [[Verse]] — one moment of dialogue. |
| 500 | [[TileMap]] | [[Any]]  | A whole combat map: a grid of tiles plus spawn points. |
| 501 | [[Pathfinding]] | [[Any]]  | Works out routes and movement costs across the map. |
| 510 | [[GridItem]] | [[Any]]  | Anything with a position on the combat grid. |
| 511 | [[PathNode]] | [[GridItem]]  | One square of the map as pathfinding sees it. |
| 512 | [[Tile]] | [[GridItem]]  | A single square of the combat map. |
| 513 | [[Unit]] | [[GridItem]]  | A character as it appears on the combat grid. |
| 520 | [[Targeting]] | [[Any]]  | The rules for how an effect picks its targets. |
| 521 | [[Target]] | [[GridItem]]  | One thing an effect was aimed at, plus its area. |
| 522 | [[TargetingResult]] | [[Any]]  | The full outcome of a targeting step — the chosen targets. |
| 530 | [[Movement]] | [[Any]]  | A single move a unit makes across the grid. |
| 1000 | [[Vector2D]] | [[Any]]  | A pair of numbers: a 2D point or direction. |
| 1001 | [[Vector3D]] | [[Any]]  | A trio of numbers: a 3D point or direction. |
| 1100 | [[AnimationListener]] | [[Any]]  | Runs script callbacks at key moments of an animation. |
| 1101 | [[CharacterVisuals]] | [[AnimationListener]]  | A character's on-screen visuals: animations and floating text. |
| 1102 | [[UnitVisuals]] | [[CharacterVisuals]]  | A unit's visuals on the combat grid. |
| 1110 | [[Projectile]] | [[Any]]  | A moving visual fired between two points in combat. |


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

