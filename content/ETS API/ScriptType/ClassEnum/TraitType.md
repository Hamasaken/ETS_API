---
title: TraitType
draft: false
tags:
 - ScriptType
 - ClassEnum
 - ScriptObject
---
# TraitType : [[ClassEnum]]

The individual traits a [[Character]] or [[Item]] can have — Human, Undead, Weapon, Fire, and so on. Traits are arranged in a hierarchy (each may have a broader parent) and belong to a [[TraitGroup]]. New traits are loaded from asset files, where each trait's own description is set.

## Enum values
| Id     | Name             | Parent         | Trait group                              | Description                                                                        |
| ------ | ---------------- | -------------- | ---------------------------------------- | ---------------------------------------------------------------------------------- |
| 10 | [[Item]] |  | [[TraitGroup#^general\|General]]  | This is a General trait. |
| 11 | [[Equipment]] | [[Item]] | [[TraitGroup#^general\|General]]  | A specific type of Item. |
| 12 | [[Consumable]] | [[Item]] | [[TraitGroup#^general\|General]]  | A specific type of Item. |
| 13 | [[Utility]] | [[Item]] | [[TraitGroup#^general\|General]]  | A specific type of Item. |
| 14 | [[Treasure]] | [[Item]] | [[TraitGroup#^general\|General]]  | A specific type of Item. |
| 20 | [[Food]] | [[Consumable]] | [[TraitGroup#^general\|General]]  | A specific type of Consumable. |
| 21 | [[Drink]] | [[Food]] | [[TraitGroup#^general\|General]]  | A specific type of Food. |
| 40 | [[Weapon]] | [[Equipment]] | [[TraitGroup#^general\|General]]  | A specific type of Equipment. |
| 41 | [[Armor]] | [[Equipment]] | [[TraitGroup#^general\|General]]  | A specific type of Equipment. |
| 42 | [[Relic]] | [[Equipment]] | [[TraitGroup#^general\|General]]  | A specific type of Equipment. |
| 100 | [[Minion]] |  | [[TraitGroup#^general\|General]]  | This is a General trait. |
| 1000 | [[Humanoid]] |  | [[TraitGroup#^race\|Race]]  | This is a Race trait. |
| 1001 | [[Human]] | [[Humanoid]] | [[TraitGroup#^race\|Race]]  | A specific type of Humanoid. |
| 1002 | [[Elf]] | [[Humanoid]] | [[TraitGroup#^race\|Race]]  | A specific type of Humanoid. |
| 1003 | [[Orc]] | [[Humanoid]] | [[TraitGroup#^race\|Race]]  | A specific type of Humanoid. |
| 1120 | [[Lamia]] |  | [[TraitGroup#^race\|Race]]  | This is a Race trait. |
| 1300 | [[Beast]] |  | [[TraitGroup#^race\|Race]]  | This is a Race trait. |
| 2000 | [[Pirate]] |  | [[TraitGroup#^job\|Job]]  | This is a Job trait. |
| 2002 | [[Necromancer]] |  | [[TraitGroup#^job\|Job]]  | This is a Job trait. |
| 2003 | [[Nun]] |  | [[TraitGroup#^job\|Job]]  | This is a Job trait. |
| 3000 | [[Curious]] |  | [[TraitGroup#^personality\|Personality]]  | This is a Personality trait. |
| 3001 | [[Conservative]] |  | [[TraitGroup#^personality\|Personality]]  | This is a Personality trait. |
| 3002 | [[Shy]] |  | [[TraitGroup#^personality\|Personality]]  | This is a Personality trait. |
| 3003 | [[Extroverted]] |  | [[TraitGroup#^personality\|Personality]]  | This is a Personality trait. |
| 3004 | [[Brave]] |  | [[TraitGroup#^personality\|Personality]]  | This is a Personality trait. |
| 3005 | [[Craven]] |  | [[TraitGroup#^personality\|Personality]]  | This is a Personality trait. |
| 4000 | [[Male]] |  | [[TraitGroup#^physical\|Physical]]  | This is a Physical trait. |
| 4001 | [[Female]] |  | [[TraitGroup#^physical\|Physical]]  | This is a Physical trait. |
| 4002 | [[Beautiful]] |  | [[TraitGroup#^physical\|Physical]]  | This is a Physical trait. |
| 4003 | [[Strong]] |  | [[TraitGroup#^physical\|Physical]]  | This is a Physical trait. |
| 5000 | [[Void]] |  | [[TraitGroup#^element\|Element]]  | This is a Element trait. |
| 5001 | [[Physical]] |  | [[TraitGroup#^element\|Element]]  | This is a Element trait. |
| 5002 | [[Fire]] |  | [[TraitGroup#^element\|Element]]  | This is a Element trait. |
| 5003 | [[Frost]] |  | [[TraitGroup#^element\|Element]]  | This is a Element trait. |
| 5004 | [[Nature]] |  | [[TraitGroup#^element\|Element]]  | This is a Element trait. |
| 5005 | [[Holy]] |  | [[TraitGroup#^element\|Element]]  | This is a Element trait. |
| 5006 | [[Necrotic]] |  | [[TraitGroup#^element\|Element]]  | This is a Element trait. |
| 5007 | [[Electric]] |  | [[TraitGroup#^element\|Element]]  | This is a Element trait. |
| 6000 | [[Buff]] |  | [[TraitGroup#^status\|Status]]  | This is a Status trait. |
| 6001 | [[Debuff]] |  | [[TraitGroup#^status\|Status]]  | This is a Status trait. |
| 100000 | [[Undead]] |  | [[TraitGroup#^race\|Race]]  | A creature of the dead somehow still wandering the land. Takes double holy damage. |
| 100001 | [[Skeleton]] | [[Undead]] | [[TraitGroup#^race\|Race]]  | Spooky and scary. |
| 100002 | [[Zombie]] | [[Undead]] | [[TraitGroup#^race\|Race]]  | The walking dead. |
| 100003 | [[Potion]] | [[Utility]] | [[TraitGroup#^general\|General]]  | An alchemical concoction in a glass bottle. |
| 100004 | [[Poison]] | [[Debuff]] | [[TraitGroup#^status\|Status]]  | A substance with harmful effects. |
| 100005 | [[Cursed]] |  | [[TraitGroup#^general\|General]]  | This character is cursed. |
| 100006 | [[Assassin]] |  | [[TraitGroup#^job\|Job]]  | Prefers to face enemies one on one. |
| 100007 | [[Buxom]] |  | [[TraitGroup#^physical\|Physical]]  | This character has a rather ample bosom. |



## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| group | [[TraitGroup]] | True | The trait group this trait belongs to. |
| parent | [[TraitType]] | True | The broader trait this one is a specific kind of, if any. |

## Script variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| OnApply | [[Function]] | False | Runs when the trait is applied to a character. |
| OnRemove | [[Function]] | False | Runs when the trait is removed from a character. |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Script functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |


