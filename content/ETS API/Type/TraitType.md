---
title: TraitType
draft: false
tags:
 - ClassEnum
 - ScriptObject
---

Description goes here.

## Values
| Id  | Name | Group | Parent | Description |
| --- | ---- | ----- | ------ | ----------- |
| 10 | [[Item]] | [[TraitGroup#^general\|General]] |   | This is a General trait. |
| 11 | [[Equipment]] | [[TraitGroup#^general\|General]] | [[Item]]  | A specific type of Item. |
| 12 | [[Consumable]] | [[TraitGroup#^general\|General]] | [[Item]]  | A specific type of Item. |
| 13 | [[Utility]] | [[TraitGroup#^general\|General]] | [[Item]]  | A specific type of Item. |
| 14 | [[Treasure]] | [[TraitGroup#^general\|General]] | [[Item]]  | A specific type of Item. |
| 20 | [[Food]] | [[TraitGroup#^general\|General]] | [[Consumable]]  | A specific type of Consumable. |
| 21 | [[Drink]] | [[TraitGroup#^general\|General]] | [[Food]]  | A specific type of Food. |
| 40 | [[Weapon]] | [[TraitGroup#^general\|General]] | [[Equipment]]  | A specific type of Equipment. |
| 41 | [[Armor]] | [[TraitGroup#^general\|General]] | [[Equipment]]  | A specific type of Equipment. |
| 42 | [[Relic]] | [[TraitGroup#^general\|General]] | [[Equipment]]  | A specific type of Equipment. |
| 100 | [[Minion]] | [[TraitGroup#^general\|General]] |   | This is a General trait. |
| 1000 | [[Humanoid]] | [[TraitGroup#^race\|Race]] |   | This is a Race trait. |
| 1001 | [[Human]] | [[TraitGroup#^race\|Race]] | [[Humanoid]]  | A specific type of Humanoid. |
| 1002 | [[Elf]] | [[TraitGroup#^race\|Race]] | [[Humanoid]]  | A specific type of Humanoid. |
| 1003 | [[Orc]] | [[TraitGroup#^race\|Race]] | [[Humanoid]]  | A specific type of Humanoid. |
| 1120 | [[Lamia]] | [[TraitGroup#^race\|Race]] |   | This is a Race trait. |
| 1300 | [[Beast]] | [[TraitGroup#^race\|Race]] |   | This is a Race trait. |
| 2000 | [[Pirate]] | [[TraitGroup#^job\|Job]] |   | This is a Job trait. |
| 2002 | [[Necromancer]] | [[TraitGroup#^job\|Job]] |   | This is a Job trait. |
| 2003 | [[Nun]] | [[TraitGroup#^job\|Job]] |   | This is a Job trait. |
| 3000 | [[Curious]] | [[TraitGroup#^personality\|Personality]] |   | This is a Personality trait. |
| 3001 | [[Conservative]] | [[TraitGroup#^personality\|Personality]] |   | This is a Personality trait. |
| 3002 | [[Shy]] | [[TraitGroup#^personality\|Personality]] |   | This is a Personality trait. |
| 3003 | [[Extroverted]] | [[TraitGroup#^personality\|Personality]] |   | This is a Personality trait. |
| 3004 | [[Brave]] | [[TraitGroup#^personality\|Personality]] |   | This is a Personality trait. |
| 3005 | [[Craven]] | [[TraitGroup#^personality\|Personality]] |   | This is a Personality trait. |
| 4000 | [[Male]] | [[TraitGroup#^physical\|Physical]] |   | This is a Physical trait. |
| 4001 | [[Female]] | [[TraitGroup#^physical\|Physical]] |   | This is a Physical trait. |
| 4002 | [[Beautiful]] | [[TraitGroup#^physical\|Physical]] |   | This is a Physical trait. |
| 4003 | [[Strong]] | [[TraitGroup#^physical\|Physical]] |   | This is a Physical trait. |
| 5000 | [[Void]] | [[TraitGroup#^element\|Element]] |   | This is a Element trait. |
| 5001 | [[Physical]] | [[TraitGroup#^element\|Element]] |   | This is a Element trait. |
| 5002 | [[Fire]] | [[TraitGroup#^element\|Element]] |   | This is a Element trait. |
| 5003 | [[Frost]] | [[TraitGroup#^element\|Element]] |   | This is a Element trait. |
| 5004 | [[Nature]] | [[TraitGroup#^element\|Element]] |   | This is a Element trait. |
| 5005 | [[Holy]] | [[TraitGroup#^element\|Element]] |   | This is a Element trait. |
| 5006 | [[Necrotic]] | [[TraitGroup#^element\|Element]] |   | This is a Element trait. |
| 5007 | [[Electric]] | [[TraitGroup#^element\|Element]] |   | This is a Element trait. |
| 6000 | [[Buff]] | [[TraitGroup#^status\|Status]] |   | This is a Status trait. |
| 6001 | [[Debuff]] | [[TraitGroup#^status\|Status]] |   | This is a Status trait. |
| 100000 | [[Undead]] | [[TraitGroup#^race\|Race]] |   | A creature of the dead somehow still wandering the land. Takes double holy damage. |
| 100001 | [[Skeleton]] | [[TraitGroup#^race\|Race]] | [[Undead]]  | Spooky and scary. |
| 100002 | [[Zombie]] | [[TraitGroup#^race\|Race]] | [[Undead]]  | The walking dead. |
| 100003 | [[Potion]] | [[TraitGroup#^general\|General]] | [[Utility]]  | An alchemical concoction in a glass bottle. |
| 100004 | [[Poison]] | [[TraitGroup#^status\|Status]] | [[Debuff]]  | A substance with harmful effects. |
| 100005 | [[Cursed]] | [[TraitGroup#^general\|General]] |   | This character is cursed. |
| 100006 | [[Assassin]] | [[TraitGroup#^job\|Job]] |   | Prefers to face enemies one on one. |
| 100007 | [[Buxom]] | [[TraitGroup#^physical\|Physical]] |   | This character has a rather ample bosom. |

## Variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| group | [[TraitGroup]] | True |  |
| parent | [[TraitType]] | True |  |

## Functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[TraitType#^onapply\|OnApply()]] | [[Void]] | [[Character]] c, [[Trait]] t |  |
| [[TraitType#^onremove\|OnRemove()]] | [[Void]] | [[Character]] c, [[Trait]] t |  |

### OnApply ([[Character]] c, [[Trait]] t) : [[Void]]

^onapply

Description goes here.

> [!Abstract]+ Parameters
> 1. `c` This is a parameter.
> 2. `t` This is a parameter.

### OnRemove ([[Character]] c, [[Trait]] t) : [[Void]]

^onremove

Description goes here.

> [!Abstract]+ Parameters
> 1. `c` This is a parameter.
> 2. `t` This is a parameter.

