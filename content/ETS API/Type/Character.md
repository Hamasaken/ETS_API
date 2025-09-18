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
| unit | [[Unit]] | True |  |
| eventImage | [[String]] | False |  |
| combatImage | [[String]] | False |  |

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
| [[Character#^getstatus\|GetStatus()]] | [[Status]] | [[String]] id |  |
| [[Character#^addstatus\|AddStatus()]] | [[Bool]] | [[Status]] status |  |
| [[Character#^removestatus\|RemoveStatus()]] | [[Bool]] | [[Status]] status |  |
| [[Character#^gethitchance\|GetHitChance()]] | [[Float]] | [[Attack]] attack |  |
| [[Character#^getevadechance\|GetEvadeChance()]] | [[Float]] |  |  |
| [[Character#^attack\|Attack()]] | [[Bool]] | [[Character]] target, [[Attack]] attack, [[Damage]] damage |  |
| [[Character#^attacktarget\|AttackTarget()]] | [[List]]<[[Character]]> | [[Target]] target, [[Attack]] attack, [[Damage]] damage |  |
| [[Character#^attacktargets\|AttackTargets()]] | [[List]]<[[Character]]> | [[List]]<[[Target]]> targets, [[Attack]] attack, [[Damage]] damage |  |
| [[Character#^takedamage\|TakeDamage()]] | [[Void]] | [[Damage]] damage |  |
| [[Character#^takedamage2\|TakeDamage2()]] | [[Void]] | [[Int]] value, [[DamageType]] type, [[Bool]] pen |  |
| [[Character#^healdamage\|HealDamage()]] | [[Void]] | [[Int]] value |  |
| [[Character#^scaledvalue\|ScaledValue()]] | [[Int]] | [[StatType]] stat, [[Float]] multiplier |  |

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

### GetStatus ([[String]] id) : [[Status]]

^getstatus

Description goes here.

> [!Abstract]+ Parameters
> 1. `id` This is a parameter.

> [!Success]+ Return value
> Returns a [[StatusEffect]].

### AddStatus ([[Status]] status) : [[Bool]]

^addstatus

Description goes here.

> [!Abstract]+ Parameters
> 1. `status` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### RemoveStatus ([[Status]] status) : [[Bool]]

^removestatus

Description goes here.

> [!Abstract]+ Parameters
> 1. `status` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

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

### Attack ([[Character]] target, [[Attack]] attack, [[Damage]] damage) : [[Bool]]

^attack

Description goes here.

> [!Abstract]+ Parameters
> 1. `target` This is a parameter.
> 2. `attack` This is a parameter.
> 3. `damage` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### AttackTarget ([[Target]] target, [[Attack]] attack, [[Damage]] damage) : [[List]]<[[Character]]>

^attacktarget

Description goes here.

> [!Abstract]+ Parameters
> 1. `target` This is a parameter.
> 2. `attack` This is a parameter.
> 3. `damage` This is a parameter.

> [!Success]+ Return value
> Returns a [[List]]<[[Character]]>.

### AttackTargets ([[List]]<[[Target]]> targets, [[Attack]] attack, [[Damage]] damage) : [[List]]<[[Character]]>

^attacktargets

Description goes here.

> [!Abstract]+ Parameters
> 1. `targets` This is a parameter.
> 2. `attack` This is a parameter.
> 3. `damage` This is a parameter.

> [!Success]+ Return value
> Returns a [[List]]<[[Character]]>.

### TakeDamage ([[Damage]] damage) : [[Void]]

^takedamage

Description goes here.

> [!Abstract]+ Parameters
> 1. `damage` This is a parameter.

### TakeDamage2 ([[Int]] value, [[DamageType]] type, [[Bool]] pen) : [[Void]]

^takedamage2

Description goes here.

> [!Abstract]+ Parameters
> 1. `value` This is a parameter.
> 2. `type` This is a parameter.
> 3. `pen` This is a parameter.

### HealDamage ([[Int]] value) : [[Void]]

^healdamage

Description goes here.

> [!Abstract]+ Parameters
> 1. `value` This is a parameter.

### ScaledValue ([[StatType]] stat, [[Float]] multiplier) : [[Int]]

^scaledvalue

Description goes here.

> [!Abstract]+ Parameters
> 1. `stat` This is a parameter.
> 2. `multiplier` This is a parameter.

> [!Success]+ Return value
> Returns a [[Int]].

