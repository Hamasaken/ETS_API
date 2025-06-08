---
title: TraitType
draft: false
tags:
  - ClassEnum
  - ScriptObject
---

Placeholder description for TraitType.

## Values
| Id   | Name             | Group                      | Parent         | Description                  |
| ---- | ---------------- | -------------------------- | -------------- | ---------------------------- |
| 10 | [[Item]] | [[TraitGroup#General]] |   | This is a General trait. |
| 11 | [[Consumable]] | [[TraitGroup#General]] | [[Item]]  | This is a General trait. |
| 12 | [[Food]] | [[TraitGroup#General]] | [[Consumable]]  | This is a General trait. |
| 13 | [[Fruit]] | [[TraitGroup#General]] | [[Food]]  | This is a General trait. |
| 100 | [[Minion]] | [[TraitGroup#General]] |   | This is a General trait. |
| 1000 | [[Humanoid]] | [[TraitGroup#Race]] |   | This is a Race trait. |
| 1001 | [[Human]] | [[TraitGroup#Race]] | [[Humanoid]]  | This is a Race trait. |
| 1002 | [[Elf]] | [[TraitGroup#Race]] | [[Humanoid]]  | This is a Race trait. |
| 1003 | [[Orc]] | [[TraitGroup#Race]] | [[Humanoid]]  | This is a Race trait. |
| 1120 | [[Lamia]] | [[TraitGroup#Race]] |   | This is a Race trait. |
| 1300 | [[Beast]] | [[TraitGroup#Race]] |   | This is a Race trait. |
| 2000 | [[Pirate]] | [[TraitGroup#Job]] |   | This is a Job trait. |
| 2002 | [[Necromancer]] | [[TraitGroup#Job]] |   | This is a Job trait. |
| 2003 | [[Nun]] | [[TraitGroup#Job]] |   | This is a Job trait. |
| 3000 | [[Curious]] | [[TraitGroup#Personality]] |   | This is a Personality trait. |
| 3001 | [[Conservative]] | [[TraitGroup#Personality]] |   | This is a Personality trait. |
| 3002 | [[Shy]] | [[TraitGroup#Personality]] |   | This is a Personality trait. |
| 3003 | [[Extroverted]] | [[TraitGroup#Personality]] |   | This is a Personality trait. |
| 3004 | [[Brave]] | [[TraitGroup#Personality]] |   | This is a Personality trait. |
| 3005 | [[Craven]] | [[TraitGroup#Personality]] |   | This is a Personality trait. |
| 4000 | [[Male]] | [[TraitGroup#Physical]] |   | This is a Physical trait. |
| 4001 | [[Female]] | [[TraitGroup#Physical]] |   | This is a Physical trait. |
| 4002 | [[Beautiful]] | [[TraitGroup#Physical]] |   | This is a Physical trait. |
| 4003 | [[Strong]] | [[TraitGroup#Physical]] |   | This is a Physical trait. |
| 5000 | [[Void]] | [[TraitGroup#Element]] |   | This is a Element trait. |
| 5001 | [[Physical]] | [[TraitGroup#Element]] |   | This is a Element trait. |
| 5002 | [[Fire]] | [[TraitGroup#Element]] |   | This is a Element trait. |
| 5003 | [[Frost]] | [[TraitGroup#Element]] |   | This is a Element trait. |
| 5004 | [[Nature]] | [[TraitGroup#Element]] |   | This is a Element trait. |
| 5005 | [[Holy]] | [[TraitGroup#Element]] |   | This is a Element trait. |
| 5006 | [[Necrotic]] | [[TraitGroup#Element]] |   | This is a Element trait. |
| 5007 | [[Electric]] | [[TraitGroup#Element]] |   | This is a Element trait. |
| 6000 | [[Buff]] | [[TraitGroup#Status]] |   | This is a Status trait. |
| 6200 | [[Debuff]] | [[TraitGroup#Status]] |   | This is a Status trait. |
| 6201 | [[Poison]] | [[TraitGroup#Status]] | [[Debuff]]  | This is a Status trait. |
| 100000 | [[Undead]] | [[TraitGroup#Race]] |   | This is a Race trait. |
| 100001 | [[Skeleton]] | [[TraitGroup#Race]] | [[Undead]]  | This is a Race trait. |
| 100002 | [[Zombie]] | [[TraitGroup#Race]] | [[Undead]]  | This is a Race trait. |

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

