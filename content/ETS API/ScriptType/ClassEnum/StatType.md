---
title: StatType
draft: false
tags:
 - ScriptType
 - ClassEnum
---
# StatType : [[ClassEnum]]

Every character in the game has a set of statistics that determines their gameplay characteristics.

## Enum values
| Id  | Name   | Default value | Description |
| ------ | ---------------------------------------- | ----- | ----- |
| 0 | [[StatType#^health\|Health]] | 10 | Maximum Health. When a character's Health pool empties, they die. |
| 1 | [[StatType#^mana\|Mana]] | 0 | Maximum Mana, spent to use abilities. |
| 2 | [[StatType#^speed\|Speed]] | 15 | Decides turn order in combat — faster units act first. |
| 3 | [[StatType#^movement\|Movement]] | 35 | Movement points per combat turn, spent on tile costs while moving. |
| 4 | [[StatType#^actions\|Actions]] | 1 | How many actions the character may take each combat turn. |
| 10 | [[StatType#^defense\|Defense]] | 0 | Subtracted from incoming damage, unless the damage penetrates. |
| 11 | [[StatType#^resistance\|Resistance]] | 0 | Not yet wired into the combat rules. |
| 12 | [[StatType#^accuracy\|Accuracy]] | 0 | Added to an attack's base accuracy when working out hit chance. |
| 13 | [[StatType#^evasiveness\|Evasiveness]] | 0 | Base chance to evade incoming attacks. |
| 100 | [[StatType#^strength\|Strength]] | 0 | Physical power; scales physical abilities. |
| 101 | [[StatType#^dexterity\|Dexterity]] | 0 | Ranged power; every 2 points add 1 to hit chance. |
| 102 | [[StatType#^intelligence\|Intelligence]] | 0 | Magical power and knowledge. |
| 103 | [[StatType#^constitution\|Constitution]] | 0 | Physical resilience; the Stamina resource scales from it. |
| 104 | [[StatType#^agility\|Agility]] | 0 | Nimbleness; every 2 points add 1 to evade chance. |
| 105 | [[StatType#^spirit\|Spirit]] | 0 | Magical resilience; scales holy and spiritual abilities. |
| 120 | [[StatType#^luck\|Luck]] | 50 | Influences random rolls, event outcomes and loot. |
| 9999 | [[StatType#^debug\|Debug]] | 0 | Used for testing; has no gameplay effect. |
| 100000 | [[StatType#^sanity\|Sanity]] | 50 | Custom stat added through the `_s1.stats` asset file. |
| 100001 | [[StatType#^schlong size\|Schlong size]] | 50 | Custom stat added through the `_s1.stats` asset file. |
