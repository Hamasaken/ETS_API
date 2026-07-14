---
title: TraitGroup
draft: false
tags:
 - ScriptType
 - ClassEnum
---
# TraitGroup : [[ClassEnum]]

Traits are organised into groups such as Race, Job or Element. A trait's group sets what its members have in common — for example whether traits of that kind are shown to the player by default. Every [[TraitType]] belongs to one TraitGroup.

## Enum values
| Id  | Name                                     | Default visibility | Description |
| --- | ---------------------------------------- | ------------------ | ----------- |
| 0 | [[TraitGroup#^general\|General]] | True | Miscellaneous traits that don't fit another group. |
| 10 | [[TraitGroup#^race\|Race]] | True | What kind of creature the character is (Human, Orc…). |
| 11 | [[TraitGroup#^job\|Job]] | False | The character's profession or class. |
| 12 | [[TraitGroup#^personality\|Personality]] | False | The character's personality. |
| 13 | [[TraitGroup#^physical\|Physical]] | True | Physical characteristics of the character. |
| 20 | [[TraitGroup#^element\|Element]] | True | Elemental affinities (Fire, Frost…). |
| 21 | [[TraitGroup#^status\|Status]] | False | Traits granted by status effects (buffs and debuffs). |


