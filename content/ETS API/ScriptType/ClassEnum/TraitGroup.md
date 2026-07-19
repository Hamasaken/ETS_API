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
| 0 | [[TraitGroup#^general\|General]] | True | Catch-all group; mostly item categories such as Equipment and Consumable. |
| 10 | [[TraitGroup#^race\|Race]] | True | What kind of creature a character is — Human, Lamia, Beast, Undead... |
| 11 | [[TraitGroup#^job\|Job]] | False | A character's profession or calling, such as Pirate or Necromancer. |
| 12 | [[TraitGroup#^personality\|Personality]] | False | A character's temperament, such as Brave or Shy. |
| 13 | [[TraitGroup#^physical\|Physical]] | True | Bodily characteristics, such as Male, Female or Strong. |
| 20 | [[TraitGroup#^element\|Element]] | True | Elemental affinities matching the damage types — Fire, Frost, Holy... |
| 21 | [[TraitGroup#^status\|Status]] | False | Categorises [[Status]] effects, e.g. as a Buff or a Debuff. |


