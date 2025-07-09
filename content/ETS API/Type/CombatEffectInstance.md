---
title: CombatEffectInstance
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

## Functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[CombatEffectInstance#^scaleddamage\|ScaledDamage()]] | [[Damage]] | [[Character]] u |  |
| [[CombatEffectInstance#^scaledvalue\|ScaledValue()]] | [[Int]] | [[Character]] u |  |
| [[CombatEffectInstance#^finish\|Finish()]] | [[Void]] |  |  |
| [[CombatEffectInstance#^spawnprojectile\|SpawnProjectile()]] | [[Projectile]] | [[GridItem]] target, [[String]] image, [[Function]] callback |  |
| [[CombatEffectInstance#^spawnprojectilec\|SpawnProjectileC()]] | [[Projectile]] | [[Character]] target, [[String]] image, [[Function]] callback |  |
| [[CombatEffectInstance#^spawnprojectileat\|SpawnProjectileAt()]] | [[Projectile]] | [[Vector3D]] spawn, [[Vector3D]] target, [[String]] image, [[Function]] callback |  |
| [[CombatEffectInstance#^queueaction\|QueueAction()]] | [[Void]] | [[AnimationListener]] listener, [[Function]] callback |  |
| [[CombatEffectInstance#^waitforanimation\|WaitForAnimation()]] | [[Void]] | [[AnimationListener]] listener, [[Function]] callback |  |
| [[CombatEffectInstance#^waitforprojectiles\|WaitForProjectiles()]] | [[Void]] | [[Function]] callback |  |
| [[CombatEffectInstance#^selecttargets\|SelectTargets()]] | [[Void]] | [[Targeting]] targeting, [[Function]] callback |  |

### ScaledDamage ([[Character]] u) : [[Damage]]

^scaleddamage

Description goes here.

> [!Abstract]+ Parameters
> 1. `u` This is a parameter.

> [!Success]+ Return value
> Returns a [[Damage]].

### ScaledValue ([[Character]] u) : [[Int]]

^scaledvalue

Description goes here.

> [!Abstract]+ Parameters
> 1. `u` This is a parameter.

> [!Success]+ Return value
> Returns a [[Int]].

### Finish () : [[Void]]

^finish

Description goes here.

### SpawnProjectile ([[GridItem]] target, [[String]] image, [[Function]] callback) : [[Projectile]]

^spawnprojectile

Description goes here.

> [!Abstract]+ Parameters
> 1. `target` This is a parameter.
> 2. `image` This is a parameter.
> 3. `callback` This is a parameter.

> [!Success]+ Return value
> Returns a [[IProjectile]].

### SpawnProjectileC ([[Character]] target, [[String]] image, [[Function]] callback) : [[Projectile]]

^spawnprojectilec

Description goes here.

> [!Abstract]+ Parameters
> 1. `target` This is a parameter.
> 2. `image` This is a parameter.
> 3. `callback` This is a parameter.

> [!Success]+ Return value
> Returns a [[IProjectile]].

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

### QueueAction ([[AnimationListener]] listener, [[Function]] callback) : [[Void]]

^queueaction

Description goes here.

> [!Abstract]+ Parameters
> 1. `listener` This is a parameter.
> 2. `callback` This is a parameter.

### WaitForAnimation ([[AnimationListener]] listener, [[Function]] callback) : [[Void]]

^waitforanimation

Description goes here.

> [!Abstract]+ Parameters
> 1. `listener` This is a parameter.
> 2. `callback` This is a parameter.

### WaitForProjectiles ([[Function]] callback) : [[Void]]

^waitforprojectiles

Description goes here.

> [!Abstract]+ Parameters
> 1. `callback` This is a parameter.

### SelectTargets ([[Targeting]] targeting, [[Function]] callback) : [[Void]]

^selecttargets

Description goes here.

> [!Abstract]+ Parameters
> 1. `targeting` This is a parameter.
> 2. `callback` This is a parameter.

