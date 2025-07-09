---
title: CombatEffect
draft: false
tags:
 - ScriptObject
---

Description goes here.

## Variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| targeting | [[Targeting]] | False |  |
| attack | [[Attack]] | False |  |
| damage | [[Damage]] | False |  |
| scaling | [[StatScaling]] | False |  |
| u | [[Character]] | True |  |
| user | [[Character]] | True |  |

## Functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[CombatEffect#^finish\|Finish()]] | [[Void]] |  |  |
| [[CombatEffect#^scaleddamage\|ScaledDamage()]] | [[Damage]] | [[Character]] u |  |
| [[CombatEffect#^selecttargets\|SelectTargets()]] | [[Void]] | [[Targeting]] targeting, [[Function]] callback |  |
| [[CombatEffect#^waitforprojectiles\|WaitForProjectiles()]] | [[Void]] | [[Function]] callback |  |
| [[CombatEffect#^spawnprojectile\|SpawnProjectile()]] | [[Projectile]] | [[GridItem]] target, [[String]] image, [[Function]] callback |  |
| [[CombatEffect#^spawnprojectileat\|SpawnProjectileAt()]] | [[Projectile]] | [[Vector3D]] spawn, [[Vector3D]] target, [[String]] image, [[Function]] callback |  |
| [[CombatEffect#^canperform\|CanPerform()]] | [[Bool]] | [[Character]] c |  |

### Finish () : [[Void]]

^finish

Description goes here.

### ScaledDamage ([[Character]] u) : [[Damage]]

^scaleddamage

Description goes here.

> [!Abstract]+ Parameters
> 1. `u` This is a parameter.

> [!Success]+ Return value
> Returns a [[Damage]].

### SelectTargets ([[Targeting]] targeting, [[Function]] callback) : [[Void]]

^selecttargets

Description goes here.

> [!Abstract]+ Parameters
> 1. `targeting` This is a parameter.
> 2. `callback` This is a parameter.

### WaitForProjectiles ([[Function]] callback) : [[Void]]

^waitforprojectiles

Description goes here.

> [!Abstract]+ Parameters
> 1. `callback` This is a parameter.

### SpawnProjectile ([[GridItem]] target, [[String]] image, [[Function]] callback) : [[Projectile]]

^spawnprojectile

Description goes here.

> [!Abstract]+ Parameters
> 1. `target` This is a parameter.
> 2. `image` This is a parameter.
> 3. `callback` This is a parameter.

> [!Success]+ Return value
> Returns a [[Projectile]].

### SpawnProjectileAt ([[Vector3D]] spawn, [[Vector3D]] target, [[String]] image, [[Function]] callback) : [[Projectile]]

^spawnprojectileat

Description goes here.

> [!Abstract]+ Parameters
> 1. `spawn` This is a parameter.
> 2. `target` This is a parameter.
> 3. `image` This is a parameter.
> 4. `callback` This is a parameter.

> [!Success]+ Return value
> Returns a [[Projectile]].

### CanPerform ([[Character]] c) : [[Bool]]

^canperform

Description goes here.

> [!Abstract]+ Parameters
> 1. `c` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

