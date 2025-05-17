---
title: Character
draft: false
tags:
 - ScriptObject
---

Description goes here.

## Variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| id | [[String]] | False |  |
| name | [[String]] | False |  |
| visuals | [[CharacterVisuals]] | True |  |
| position | [[GridItem]] | False |  |
| team | [[Team]] | False |  |

## Functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Character#^is\|Is()]] | [[Bool]] | [[FlagType]] flag |  |
| [[Character#^setflag\|SetFlag()]] | [[Void]] | [[FlagType]] flag, [[Bool]] value |  |
| [[Character#^istrait\|IsTrait()]] | [[Bool]] | [[TraitType]] trait |  |
| [[Character#^hastrait\|HasTrait()]] | [[Bool]] | [[TraitType]] trait |  |
| [[Character#^addtrait\|AddTrait()]] | [[Void]] | [[TraitType]] trait |  |
| [[Character#^removetrait\|RemoveTrait()]] | [[Void]] | [[TraitType]] trait |  |
| [[Character#^hasstat\|HasStat()]] | [[Bool]] | [[StatType]] stat |  |
| [[Character#^stat\|Stat()]] | [[Stat]] | [[StatType]] stat |  |
| [[Character#^getstat\|GetStat()]] | [[Int]] | [[StatType]] stat |  |
| [[Character#^setstat\|SetStat()]] | [[Void]] | [[StatType]] stat, [[Int]] value |  |
| [[Character#^hasstatus\|HasStatus()]] | [[Bool]] | [[String]] id |  |
| [[Character#^getstatus\|GetStatus()]] | [[StatusEffect]] | [[String]] id |  |
| [[Character#^addstatus\|AddStatus()]] | [[Bool]] | [[StatusEffect]] status |  |
| [[Character#^removestatus\|RemoveStatus()]] | [[Void]] | [[StatusEffect]] status |  |
| [[Character#^gethitchance\|GetHitChance()]] | [[Float]] | [[Attack]] attack |  |
| [[Character#^getevadechance\|GetEvadeChance()]] | [[Float]] |  |  |
| [[Character#^performattack\|PerformAttack()]] | [[Bool]] | [[Character]] target, [[Attack]] attack, [[Damage]] damage |  |
| [[Character#^takedamage\|TakeDamage()]] | [[Void]] | [[Damage]] damage |  |
| [[Character#^takedamage2\|TakeDamage2()]] | [[Void]] | [[Damage]] damage |  |
| [[Character#^healdamage\|HealDamage()]] | [[Void]] | [[Int]] value |  |
| [[Character#^changestat\|ChangeStat()]] | [[Void]] | [[StatType]] stat, [[StatAction]] action, [[Int]] value |  |
| [[Character#^isally\|IsAlly()]] | [[Bool]] | [[Character]] character |  |
| [[Character#^isenemy\|IsEnemy()]] | [[Bool]] | [[Character]] character |  |

### Is ([[FlagType]] flag) : [[Bool]]

^is

Description goes here.

> [!Abstract]+ Parameters
> 1. `flag` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### SetFlag ([[FlagType]] flag, [[Bool]] value) : [[Void]]

^setflag

Description goes here.

> [!Abstract]+ Parameters
> 1. `flag` This is a parameter.
> 2. `value` This is a parameter.

### IsTrait ([[TraitType]] trait) : [[Bool]]

^istrait

Description goes here.

> [!Abstract]+ Parameters
> 1. `trait` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### HasTrait ([[TraitType]] trait) : [[Bool]]

^hastrait

Description goes here.

> [!Abstract]+ Parameters
> 1. `trait` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### AddTrait ([[TraitType]] trait) : [[Void]]

^addtrait

Description goes here.

> [!Abstract]+ Parameters
> 1. `trait` This is a parameter.

### RemoveTrait ([[TraitType]] trait) : [[Void]]

^removetrait

Description goes here.

> [!Abstract]+ Parameters
> 1. `trait` This is a parameter.

### HasStat ([[StatType]] stat) : [[Bool]]

^hasstat

Description goes here.

> [!Abstract]+ Parameters
> 1. `stat` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### Stat ([[StatType]] stat) : [[Stat]]

^stat

Description goes here.

> [!Abstract]+ Parameters
> 1. `stat` This is a parameter.

> [!Success]+ Return value
> Returns a [[Stat]].

### GetStat ([[StatType]] stat) : [[Int]]

^getstat

Description goes here.

> [!Abstract]+ Parameters
> 1. `stat` This is a parameter.

> [!Success]+ Return value
> Returns a [[Int]].

### SetStat ([[StatType]] stat, [[Int]] value) : [[Void]]

^setstat

Description goes here.

> [!Abstract]+ Parameters
> 1. `stat` This is a parameter.
> 2. `value` This is a parameter.

### HasStatus ([[String]] id) : [[Bool]]

^hasstatus

Description goes here.

> [!Abstract]+ Parameters
> 1. `id` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### GetStatus ([[String]] id) : [[StatusEffect]]

^getstatus

Description goes here.

> [!Abstract]+ Parameters
> 1. `id` This is a parameter.

> [!Success]+ Return value
> Returns a [[StatusEffect]].

### AddStatus ([[StatusEffect]] status) : [[Bool]]

^addstatus

Description goes here.

> [!Abstract]+ Parameters
> 1. `status` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### RemoveStatus ([[StatusEffect]] status) : [[Void]]

^removestatus

Description goes here.

> [!Abstract]+ Parameters
> 1. `status` This is a parameter.

### GetHitChance ([[Attack]] attack) : [[Float]]

^gethitchance

Description goes here.

> [!Abstract]+ Parameters
> 1. `attack` This is a parameter.

> [!Success]+ Return value
> Returns a [[Float]].

### GetEvadeChance () : [[Float]]

^getevadechance

Description goes here.

> [!Success]+ Return value
> Returns a [[Float]].

### PerformAttack ([[Character]] target, [[Attack]] attack, [[Damage]] damage) : [[Bool]]

^performattack

Makes this character attempt to attack a target character using the [[Attack]] values.
If the attack hits, and the damage parameter has been set, then the game also deals the damage to the target.

> [!Abstract]+ Parameters
> 1. `target` This is a parameter.
> 2. `attack` Settings for hitchance and [[AttackType]].
> 3. `damage` Settings for damage amount and [[DamageType]].

> [!Success]+ Return value
> Returns a [[Bool]].

### TakeDamage ([[Damage]] damage) : [[Void]]

^takedamage

Description goes here.

> [!Abstract]+ Parameters
> 1. `damage` This is a parameter.

### TakeDamage2 ([[Damage]] damage) : [[Void]]

^takedamage2

Description goes here.

> [!Abstract]+ Parameters
> 1. `damage` This is a parameter.

### HealDamage ([[Int]] value) : [[Void]]

^healdamage

Description goes here.

> [!Abstract]+ Parameters
> 1. `value` This is a parameter.

### ChangeStat ([[StatType]] stat, [[StatAction]] action, [[Int]] value) : [[Void]]

^changestat

Description goes here.

> [!Abstract]+ Parameters
> 1. `stat` This is a parameter.
> 2. `action` This is a parameter.
> 3. `value` This is a parameter.

### IsAlly ([[Character]] character) : [[Bool]]

^isally

Description goes here.

> [!Abstract]+ Parameters
> 1. `character` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### IsEnemy ([[Character]] character) : [[Bool]]

^isenemy

Description goes here.

> [!Abstract]+ Parameters
> 1. `character` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

