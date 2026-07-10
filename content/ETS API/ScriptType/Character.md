---
title: Character
draft: false
tags:
 - ScriptType
---
# Character : [[BaseAsset]]

Description goes here.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| visuals | [[UnitVisuals]] | True |  |
| unit | [[Unit]] | True |  |
| eventImage | [[String]] | False |  |
| combatImage | [[String]] | False |  |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Character#^is-535570564\|Is()]] | [[Bool]] | [[FlagType]] flag |  |
| [[Character#^setflag-142902377\|SetFlag()]] | [[Void]] | [[FlagType]] flag, [[Bool]] value |  |
| [[Character#^istrait75900597\|IsTrait()]] | [[Bool]] | [[TraitType]] trait |  |
| [[Character#^hastrait-1892446971\|HasTrait()]] | [[Bool]] | [[TraitType]] trait |  |
| [[Character#^addtrait-1987476510\|AddTrait()]] | [[Void]] | [[TraitType]] trait |  |
| [[Character#^removetrait-1254612727\|RemoveTrait()]] | [[Void]] | [[TraitType]] trait |  |
| [[Character#^hasstat1719545810\|HasStat()]] | [[Bool]] | [[StatType]] stat |  |
| [[Character#^stat2125608822\|Stat()]] | [[Stat]] | [[StatType]] stat |  |
| [[Character#^hasstatus913915793\|HasStatus()]] | [[Bool]] | [[String]] id |  |
| [[Character#^getstatus952185405\|GetStatus()]] | [[Status]] | [[String]] id |  |
| [[Character#^addstatus608629884\|AddStatus()]] | [[Bool]] | [[Status]] status |  |
| [[Character#^removestatus429380083\|RemoveStatus()]] | [[Bool]] | [[Status]] status |  |
| [[Character#^gethitchance1278241276\|GetHitChance()]] | [[Float]] | [[Attack]] attack |  |
| [[Character#^getevadechance31744674\|GetEvadeChance()]] | [[Float]] |  |  |
| [[Character#^attack-1683494812\|Attack()]] | [[Bool]] | [[Character]] target, [[Attack]] attack, \[[[Damage]] damage\] |  |
| [[Character#^attack-1674229811\|Attack()]] | [[List]]<[[Character]]> | [[Target]] target, [[Attack]] attack, \[[[Damage]] damage\] |  |
| [[Character#^attack-1169034033\|Attack()]] | [[List]]<[[Character]]> | [[List]]<[[Target]]> targets, [[Attack]] attack, \[[[Damage]] damage\] |  |
| [[Character#^takedamage-638525238\|TakeDamage()]] | [[Void]] | [[Damage]] damage |  |
| [[Character#^takedamage551244711\|TakeDamage()]] | [[Void]] | [[Int]] value, [[DamageType]] type, \[[[Bool]] pen\] |  |
| [[Character#^healdamage-1787536189\|HealDamage()]] | [[Void]] | [[Int]] value |  |
| [[Character#^scaledvalue1828505233\|ScaledValue()]] | [[Int]] | [[StatType]] stat, [[Float]] multiplier |  |
| [[Character#^restore2014170150\|Restore()]] | [[Void]] | [[String]] stat, [[Int]] value | |
| [[Character#^getpercent-1964018478\|GetPercent()]] | [[Float]] | [[String]] stat | |
| [[Character#^getresource169960115\|GetResource()]] | [[Int]] | [[String]] stat | |



### Is ([[FlagType]] flag) : [[Bool]]

^is-535570564

This is a function.

> [!Abstract]+ Parameters
> 1. `flag` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### SetFlag ([[FlagType]] flag, [[Bool]] value) : [[Void]]

^setflag-142902377

This is a function.

> [!Abstract]+ Parameters
> 1. `flag` This is a parameter.
> 2. `value` This is a parameter.

### IsTrait ([[TraitType]] trait) : [[Bool]]

^istrait75900597

This is a function.

> [!Abstract]+ Parameters
> 1. `trait` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### HasTrait ([[TraitType]] trait) : [[Bool]]

^hastrait-1892446971

This is a function.

> [!Abstract]+ Parameters
> 1. `trait` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### AddTrait ([[TraitType]] trait) : [[Void]]

^addtrait-1987476510

This is a function.

> [!Abstract]+ Parameters
> 1. `trait` This is a parameter.

### RemoveTrait ([[TraitType]] trait) : [[Void]]

^removetrait-1254612727

This is a function.

> [!Abstract]+ Parameters
> 1. `trait` This is a parameter.

### HasStat ([[StatType]] stat) : [[Bool]]

^hasstat1719545810

This is a function.

> [!Abstract]+ Parameters
> 1. `stat` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### Stat ([[StatType]] stat) : [[Stat]]

^stat2125608822

This is a function.

> [!Abstract]+ Parameters
> 1. `stat` This is a parameter.

> [!Success]+ Return value
> Returns a [[Stat]].

### HasStatus ([[String]] id) : [[Bool]]

^hasstatus913915793

This is a function.

> [!Abstract]+ Parameters
> 1. `id` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### GetStatus ([[String]] id) : [[Status]]

^getstatus952185405

This is a function.

> [!Abstract]+ Parameters
> 1. `id` This is a parameter.

> [!Success]+ Return value
> Returns a [[Status]].

### AddStatus ([[Status]] status) : [[Bool]]

^addstatus608629884

This is a function.

> [!Abstract]+ Parameters
> 1. `status` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### RemoveStatus ([[Status]] status) : [[Bool]]

^removestatus429380083

This is a function.

> [!Abstract]+ Parameters
> 1. `status` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### GetHitChance ([[Attack]] attack) : [[Float]]

^gethitchance1278241276

This is a function.

> [!Abstract]+ Parameters
> 1. `attack` This is a parameter.

> [!Success]+ Return value
> Returns a [[Float]].

### GetEvadeChance () : [[Float]]

^getevadechance31744674

This is a function.

> [!Success]+ Return value
> Returns a [[Float]].

### Attack ([[Character]] target, [[Attack]] attack, \[[[Damage]] damage\]) : [[Bool]]

^attack-1683494812

This is a function.

> [!Abstract]+ Parameters
> 1. `target` This is a parameter.
> 2. `attack` This is a parameter.
> 3. `damage` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### Attack ([[Target]] target, [[Attack]] attack, \[[[Damage]] damage\]) : [[List]]<[[Character]]>

^attack-1674229811

This is a function.

> [!Abstract]+ Parameters
> 1. `target` This is a parameter.
> 2. `attack` This is a parameter.
> 3. `damage` This is a parameter.

> [!Success]+ Return value
> Returns a [[List]]<[[Character]]>.

### Attack ([[List]]<[[Target]]> targets, [[Attack]] attack, \[[[Damage]] damage\]) : [[List]]<[[Character]]>

^attack-1169034033

This is a function.

> [!Abstract]+ Parameters
> 1. `targets` This is a parameter.
> 2. `attack` This is a parameter.
> 3. `damage` This is a parameter.

> [!Success]+ Return value
> Returns a [[List]]<[[Character]]>.

### TakeDamage ([[Damage]] damage) : [[Void]]

^takedamage-638525238

This is a function.

> [!Abstract]+ Parameters
> 1. `damage` This is a parameter.

### TakeDamage ([[Int]] value, [[DamageType]] type, \[[[Bool]] pen\]) : [[Void]]

^takedamage551244711

This is a function.

> [!Abstract]+ Parameters
> 1. `value` This is a parameter.
> 2. `type` This is a parameter.
> 3. `pen` This is a parameter.

### HealDamage ([[Int]] value) : [[Void]]

^healdamage-1787536189

This is a function.

> [!Abstract]+ Parameters
> 1. `value` This is a parameter.

### ScaledValue ([[StatType]] stat, [[Float]] multiplier) : [[Int]]

^scaledvalue1828505233

This is a function.

> [!Abstract]+ Parameters
> 1. `stat` This is a parameter.
> 2. `multiplier` This is a parameter.

> [!Success]+ Return value
> Returns a [[Int]].

### Restore ([[String]] stat, [[Int]] value) : [[Void]]

^restore2014170150

This is a function.

> [!Abstract]+ Parameters
> 1. `stat` This is a parameter.
> 2. `value` This is a parameter.

### GetPercent ([[String]] stat) : [[Float]]

^getpercent-1964018478

This is a function.

> [!Abstract]+ Parameters
> 1. `stat` This is a parameter.

> [!Success]+ Return value
> Returns a [[Float]].

### GetResource ([[String]] stat) : [[Int]]

^getresource169960115

This is a function.

> [!Abstract]+ Parameters
> 1. `stat` This is a parameter.

> [!Success]+ Return value
> Returns a [[Int]].

