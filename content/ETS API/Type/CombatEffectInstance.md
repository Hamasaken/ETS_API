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
| [[CombatEffectInstance#^scaleddamage\|ScaledDamage()]] | [[Damage]] |  |  |
| [[CombatEffectInstance#^finish\|Finish()]] | [[Void]] |  |  |
| [[CombatEffectInstance#^spawnprojectile\|SpawnProjectile()]] | [[IProjectile]] | [[Vector3D]] spawn, [[Vector3D]] target, [[String]] image, [[Function]] callback |  |
| [[CombatEffectInstance#^spawnprojectilec\|SpawnProjectileC()]] | [[IProjectile]] | [[Character]] spawn, [[Vector3D]] target, [[String]] image, [[Function]] callback |  |
| [[CombatEffectInstance#^spawnprojectilet\|SpawnProjectileT()]] | [[IProjectile]] | [[Tile]] spawn, [[Vector3D]] target, [[String]] image, [[Function]] callback |  |
| [[CombatEffectInstance#^queueaction\|QueueAction()]] | [[Void]] | [[IAnimationListener]] listener, [[Function]] callback |  |
| [[CombatEffectInstance#^waitforanimation\|WaitForAnimation()]] | [[Void]] | [[IAnimationListener]] listener, [[Function]] callback |  |
| [[CombatEffectInstance#^waitforprojectiles\|WaitForProjectiles()]] | [[Void]] | [[Function]] callback |  |
| [[CombatEffectInstance#^selecttargets\|SelectTargets()]] | [[Void]] | [[Targeting]] targeting, [[Function]] callback |  |

### ScaledDamage () : [[Damage]]

^scaleddamage

Description goes here.

> [!Success]+ Return value
> Returns a [[Damage]].

### Finish () : [[Void]]

^finish

Description goes here.

### SpawnProjectile ([[Vector3D]] spawn, [[Vector3D]] target, [[String]] image, [[Function]] callback) : [[IProjectile]]

^spawnprojectile

Description goes here.

> [!Abstract]+ Parameters
> 1. `spawn` This is a parameter.
> 2. `target` This is a parameter.
> 3. `image` This is a parameter.
> 4. `callback` This is a parameter.

> [!Success]+ Return value
> Returns a [[IProjectile]].

### SpawnProjectileC ([[Character]] spawn, [[Vector3D]] target, [[String]] image, [[Function]] callback) : [[IProjectile]]

^spawnprojectilec

Description goes here.

> [!Abstract]+ Parameters
> 1. `spawn` This is a parameter.
> 2. `target` This is a parameter.
> 3. `image` This is a parameter.
> 4. `callback` This is a parameter.

> [!Success]+ Return value
> Returns a [[IProjectile]].

### SpawnProjectileT ([[Tile]] spawn, [[Vector3D]] target, [[String]] image, [[Function]] callback) : [[IProjectile]]

^spawnprojectilet

Description goes here.

> [!Abstract]+ Parameters
> 1. `spawn` This is a parameter.
> 2. `target` This is a parameter.
> 3. `image` This is a parameter.
> 4. `callback` This is a parameter.

> [!Success]+ Return value
> Returns a [[IProjectile]].

### QueueAction ([[IAnimationListener]] listener, [[Function]] callback) : [[Void]]

^queueaction

Description goes here.

> [!Abstract]+ Parameters
> 1. `listener` This is a parameter.
> 2. `callback` This is a parameter.

### WaitForAnimation ([[IAnimationListener]] listener, [[Function]] callback) : [[Void]]

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

