---
title: Character
draft: false
tags:
 - ScriptType
---
# Character : [[BaseAsset]]

A Character is a person in the game — a party member, an enemy, or an NPC. It holds everything that defines them: their [[Stat]]s, [[Trait]]s, active [[Status]] effects, [[Ability|abilities]], flags, and their current health and mana. In combat a character appears on the grid as a [[Unit]]. Most gameplay scripting reads or changes a character through the functions here — checking traits, applying statuses, dealing and healing damage, and so on.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| visuals | [[UnitVisuals]] | True | The character's on-screen representation (floating text, animations…). |
| unit | [[Unit]] | True | The character's piece on the combat grid, when in a battle. |
| eventImage | [[String]] | False | Image shown for this character in story events. |
| combatImage | [[String]] | False | Image shown for this character during combat. |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Character#^is-535570564\|Is()]] | [[Bool]] | [[FlagType]] flag | True if a flag (like Alive) is set. |
| [[Character#^setflag-142902377\|SetFlag()]] | [[Void]] | [[FlagType]] flag, [[Bool]] value | Turns a flag on or off. |
| [[Character#^istrait75900597\|IsTrait()]] | [[Bool]] | [[TraitType]] trait | True if the character counts as having a trait (or its group). |
| [[Character#^hastrait-1892446971\|HasTrait()]] | [[Bool]] | [[TraitType]] trait | True if the character has exactly this trait. |
| [[Character#^addtrait-1987476510\|AddTrait()]] | [[Void]] | [[TraitType]] trait | Gives the character a trait. |
| [[Character#^removetrait-1254612727\|RemoveTrait()]] | [[Void]] | [[TraitType]] trait | Removes a trait from the character. |
| [[Character#^hasstat1719545810\|HasStat()]] | [[Bool]] | [[StatType]] stat | True if the character has this stat. |
| [[Character#^stat2125608822\|Stat()]] | [[Stat]] | [[StatType]] stat | Gets one of the character's stats. |
| [[Character#^addstat71813794\|AddStat()]] | [[Stat]] | [[StatType]] stat, \[[[Int]] value\] | Gives the character a new stat. |
| [[Character#^removestat228464214\|RemoveStat()]] | [[Bool]] | [[StatType]] stat | Takes a stat away, when allowed. |
| [[Character#^hasresource-1109856447\|HasResource()]] | [[Bool]] | [[ResourceType]] type | True if the character has this resource pool. |
| [[Character#^resource173890153\|Resource()]] | [[Resource]] | [[ResourceType]] type | Gets one of the character's resource pools. |
| [[Character#^addresource-1769469334\|AddResource()]] | [[Resource]] | [[ResourceType]] type | Gives the character a new resource pool. |
| [[Character#^removeresource-2027243859\|RemoveResource()]] | [[Bool]] | [[ResourceType]] type | Takes a resource pool away, when allowed. |
| [[Character#^hasstatus913915793\|HasStatus()]] | [[Bool]] | [[String]] id | True if the character has this status effect. |
| [[Character#^getstatus952185405\|GetStatus()]] | [[Status]] | [[String]] id | Finds a status effect on the character by id. |
| [[Character#^addstatus608629884\|AddStatus()]] | [[Bool]] | [[Status]] status | Applies a status effect to the character. |
| [[Character#^removestatus429380083\|RemoveStatus()]] | [[Bool]] | [[Status]] status | Removes a status effect from the character. |
| [[Character#^gethitchance1278241276\|GetHitChance()]] | [[Float]] | [[Attack]] attack | Hit chance for an attack against this character. |
| [[Character#^getevadechance31744674\|GetEvadeChance()]] | [[Float]] |  | This character's chance to evade. |
| [[Character#^attack-1683494812\|Attack()]] | [[Bool]] | [[Character]] target, [[Attack]] attack, \[[[Damage]] damage\] | Attacks another character. |
| [[Character#^attack-1674229811\|Attack()]] | [[List]]<[[Character]]> | [[Target]] target, [[Attack]] attack, \[[[Damage]] damage\] | Attacks whatever a target points at. |
| [[Character#^attack-1169034033\|Attack()]] | [[List]]<[[Character]]> | [[List]]<[[Target]]> targets, [[Attack]] attack, \[[[Damage]] damage\] | Attacks several targets at once. |
| [[Character#^takedamage-638525238\|TakeDamage()]] | [[Void]] | [[Damage]] damage | Deals a prepared damage to the character. |
| [[Character#^takedamage551244711\|TakeDamage()]] | [[Void]] | [[Int]] value, [[DamageType]] type, \[[[Bool]] pen\] | Deals a set amount of damage. |
| [[Character#^healdamage-1787536189\|HealDamage()]] | [[Void]] | [[Int]] value | Heals the character. |
| [[Character#^scaledvalue1828505233\|ScaledValue()]] | [[Int]] | [[StatType]] stat, [[Float]] multiplier | A stat value multiplied by an amount. |



### Is ([[FlagType]] flag) : [[Bool]]

^is-535570564

Checks whether a flag is currently switched on for this character, such as whether they are still alive. A flag that was never set counts as off.

> [!Abstract]+ Parameters
> 1. `flag` The flag to check.

> [!Success]+ Return value
> Returns true if the flag is on.

### SetFlag ([[FlagType]] flag, [[Bool]] value) : [[Void]]

^setflag-142902377

Turns a flag on or off for this character.

> [!Abstract]+ Parameters
> 1. `flag` The flag to change.
> 2. `value` True to turn the flag on, false to turn it off.

### IsTrait ([[TraitType]] trait) : [[Bool]]

^istrait75900597

Checks whether the character counts as having a given trait — either exactly that trait, or another one that belongs to the same trait group. To match one exact trait only, use [[Character#^hastrait-1892446971\|HasTrait()]] instead.

> [!Example]+ Example
> Only let an ability target characters that aren't undead:
> ```js
> "canTarget": "!t.c.IsTrait('Undead')"
> ```

> [!Abstract]+ Parameters
> 1. `trait` The trait (or trait group) to check for.

> [!Success]+ Return value
> Returns true if the character has the trait or one from its group.

### HasTrait ([[TraitType]] trait) : [[Bool]]

^hastrait-1892446971

Checks whether the character has exactly the given trait. Unlike [[Character#^istrait75900597\|IsTrait()]], this does not count other traits from the same group.

> [!Abstract]+ Parameters
> 1. `trait` The exact trait to check for.

> [!Success]+ Return value
> Returns true if the character has that exact trait.

### AddTrait ([[TraitType]] trait) : [[Void]]

^addtrait-1987476510

Gives the character a trait and applies its effects. Nothing happens if they already have that exact trait.

> [!Abstract]+ Parameters
> 1. `trait` The trait to give the character.

### RemoveTrait ([[TraitType]] trait) : [[Void]]

^removetrait-1254612727

Removes a trait from the character, undoing whatever effects it applied.

> [!Abstract]+ Parameters
> 1. `trait` The trait to remove.

### HasStat ([[StatType]] stat) : [[Bool]]

^hasstat1719545810

Checks whether the character has a given stat at all. Useful before reading a stat that not every character necessarily has.

> [!Abstract]+ Parameters
> 1. `stat` The stat to check for.

> [!Success]+ Return value
> Returns true if the character has that stat.

### Stat ([[StatType]] stat) : [[Stat]]

^stat2125608822

Gets one of the character's [[Stat]]s so you can read its value or change it.

> [!Abstract]+ Parameters
> 1. `stat` Which stat to get.

> [!Success]+ Return value
> Returns the character's stat of that type.

### AddStat ([[StatType]] stat, \[[[Int]] value\]) : [[Stat]]

^addstat71813794

Gives the character a new [[Stat]]. If they already have it, nothing changes and the existing stat is returned — a character's stats are never replaced. If one of the character's resources draws its maximum from this stat (like Stamina from Constitution), the two are linked up right away.

> [!Abstract]+ Parameters
> 1. `stat` The stat to give the character.
> 2. `value` The starting base value. Leave it out (or pass 0) to use the stat's default.

> [!Success]+ Return value
> Returns the new stat, or the existing one if the character already had it.

### RemoveStat ([[StatType]] stat) : [[Bool]]

^removestat228464214

Takes a stat away from the character. Essential stats (the ones every character must have) can't be removed, and neither can a stat that provides the maximum of one of the character's resources — remove that resource first.

> [!Abstract]+ Parameters
> 1. `stat` The stat to remove.

> [!Success]+ Return value
> Returns true if the stat was removed.

### HasResource ([[ResourceType]] type) : [[Bool]]

^hasresource-1109856447

Checks whether the character has a resource pool of the given type. Every character has the essential pools (Health and Mana); extra ones like Stamina only exist if something added them.

> [!Abstract]+ Parameters
> 1. `type` The kind of resource to check for.

> [!Success]+ Return value
> Returns true if the character has that resource pool.

### Resource ([[ResourceType]] type) : [[Resource]]

^resource173890153

Gets one of the character's [[Resource]] pools, so you can read how full it is or add to and take from it.

> [!Example]+ Example
> Only allow an ability while the character has more than 4 Health:
> ```js
> "canPerform": "c.Resource('Health').value > 4"
> ```

> [!Abstract]+ Parameters
> 1. `type` Which resource pool to get.

> [!Success]+ Return value
> Returns the character's resource pool of that type.

### AddResource ([[ResourceType]] type) : [[Resource]]

^addresource-1769469334

Gives the character a new [[Resource]] pool of the given type and fills it according to that type's settings. If they already have it, nothing changes and the existing pool is returned. When the pool draws its maximum from a stat the character doesn't have yet, that stat is added automatically at its default value.

> [!Abstract]+ Parameters
> 1. `type` The kind of resource pool to add.

> [!Success]+ Return value
> Returns the new resource pool, or the existing one if the character already had it.

### RemoveResource ([[ResourceType]] type) : [[Bool]]

^removeresource-2027243859

Takes a resource pool away from the character. Essential pools such as Health and Mana can't be removed.

> [!Abstract]+ Parameters
> 1. `type` The resource pool to remove.

> [!Success]+ Return value
> Returns true if the resource pool was removed.

### HasStatus ([[String]] id) : [[Bool]]

^hasstatus913915793

Checks whether the character currently has a status effect with the given id (for example a poison or a buff).

> [!Abstract]+ Parameters
> 1. `id` The id of the status effect to look for.

> [!Success]+ Return value
> Returns true if the character has that status effect.

### GetStatus ([[String]] id) : [[Status]]

^getstatus952185405

Finds a status effect on the character by its id, so you can read or change it. Gives nothing back if the character doesn't have that status.

> [!Abstract]+ Parameters
> 1. `id` The id of the status effect to fetch.

> [!Success]+ Return value
> Returns the matching status effect, or nothing if the character doesn't have it.

### AddStatus ([[Status]] status) : [[Bool]]

^addstatus608629884

Applies a status effect to the character and runs its effects. It won't be added if the character already has that same status, or if it is a unique status they already carry.

> [!Example]+ Example
> Apply a prepared status to the character that was hit:
> ```js
> c.AddStatus(s)
> ```

> [!Abstract]+ Parameters
> 1. `status` The status effect to apply.

> [!Success]+ Return value
> Returns true if the status was actually added.

### RemoveStatus ([[Status]] status) : [[Bool]]

^removestatus429380083

Removes a status effect from the character, undoing its effects.

> [!Abstract]+ Parameters
> 1. `status` The status effect to remove.

> [!Success]+ Return value
> Returns true if the character had that status and it was removed.

### GetHitChance ([[Attack]] attack) : [[Float]]

^gethitchance1278241276

Works out the hit chance for an attack against this character, combining the attack's base accuracy with this character's Accuracy stat plus half of their Dexterity. It is compared against a character's evade chance when resolving an attack.

> [!Abstract]+ Parameters
> 1. `attack` The attack whose accuracy is used.

> [!Success]+ Return value
> Returns the calculated hit chance.

### GetEvadeChance () : [[Float]]

^getevadechance31744674

Works out this character's chance to evade an attack, from their Evasiveness stat plus half of their Agility. A higher value makes them harder to hit.

> [!Success]+ Return value
> Returns the character's evade chance.

### Attack ([[Character]] target, [[Attack]] attack, \[[[Damage]] damage\]) : [[Bool]]

^attack-1683494812

Makes this character attack another one, rolling to hit against the target's evade chance. If the attack lands and a damage is supplied, the target takes that damage.

> [!Example]+ Example
> Attack the target and, only on a hit, deal scaled damage:
> ```js
> if (u.Attack(c, attack)) { c.TakeDamage(ScaledDamage(u)); }
> ```

> [!Abstract]+ Parameters
> 1. `target` The character being attacked.
> 2. `attack` The attack being used, which sets the accuracy.
> 3. `damage` Damage to deal if the attack hits. Leave out to only test the hit.

> [!Success]+ Return value
> Returns true if the attack hit.

### Attack ([[Target]] target, [[Attack]] attack, \[[[Damage]] damage\]) : [[List]]<[[Character]]>

^attack-1674229811

Attacks whatever a [[Target]] points at — a single unit, or every unit in an area — rolling to hit each one and dealing the optional damage to those that are hit.

> [!Example]+ Example
> Attack everything a target covers and act on each character hit:
> ```js
> var hits = u.Attack(t, attack);
> ```

> [!Abstract]+ Parameters
> 1. `target` What to attack (a single unit or an area of units).
> 2. `attack` The attack being used, which sets the accuracy.
> 3. `damage` Damage to deal to each character that is hit. Leave out to only test the hits.

> [!Success]+ Return value
> Returns the list of characters that were hit.

### Attack ([[List]]<[[Target]]> targets, [[Attack]] attack, \[[[Damage]] damage\]) : [[List]]<[[Character]]>

^attack-1169034033

Attacks several [[Target]]s at once, rolling to hit every unit each one covers and dealing the optional damage to those that are hit.

> [!Example]+ Example
> Attack a whole list of targets and collect everyone hit:
> ```js
> var hits = u.Attack(targets, attack);
> ```

> [!Abstract]+ Parameters
> 1. `targets` The list of targets to attack.
> 2. `attack` The attack being used, which sets the accuracy.
> 3. `damage` Damage to deal to each character that is hit. Leave out to only test the hits.

> [!Success]+ Return value
> Returns the list of every character that was hit.

### TakeDamage ([[Damage]] damage) : [[Void]]

^takedamage-638525238

Deals a prepared [[Damage]] to the character. Unless the damage penetrates, the character's Defense reduces it first; any amount left over lowers their health.

> [!Abstract]+ Parameters
> 1. `damage` The damage to deal.

### TakeDamage ([[Int]] value, [[DamageType]] type, \[[[Bool]] pen\]) : [[Void]]

^takedamage551244711

Deals a set amount of damage of a given type to the character — a shortcut for building a [[Damage]] yourself. Turn on penetration to bypass their Defense.

> [!Example]+ Example
> Deal poison damage each tick, ignoring armour:
> ```js
> "onTick": "c.TakeDamage(damage, damageType, true);"
> ```

> [!Abstract]+ Parameters
> 1. `value` How much damage to deal.
> 2. `type` The kind of damage (Physical, Fire, and so on).
> 3. `pen` True to ignore the character's Defense. Leave out for normal, armour-reduced damage.

### HealDamage ([[Int]] value) : [[Void]]

^healdamage-1787536189

Heals the character by removing that much accumulated damage, restoring health up to (but never above) their maximum.

> [!Abstract]+ Parameters
> 1. `value` How much health to restore.

### ScaledValue ([[StatType]] stat, [[Float]] multiplier) : [[Int]]

^scaledvalue1828505233

Takes one of the character's stat values, multiplies it by the given amount, and rounds down to a whole number. Handy for effects that scale with a stat, such as damage or healing based on Strength.

> [!Example]+ Example
> Add healing that scales with a stat:
> ```js
> hp += u.ScaledValue(scalingStat, scalingMulti);
> ```

> [!Abstract]+ Parameters
> 1. `stat` Which stat's value to scale.
> 2. `multiplier` The amount to multiply the stat value by.

> [!Success]+ Return value
> Returns the scaled value, rounded down to a whole number.

