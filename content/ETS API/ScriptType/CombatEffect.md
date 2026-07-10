---
title: CombatEffect
draft: false
tags:
 - ScriptType
 - ScriptObject
---
# CombatEffect : [[Any]]

Description goes here.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| targeting | [[Targeting]] | False |  |
| attack | [[Attack]] | False |  |
| damage | [[Damage]] | False |  |
| scaling | [[StatScaling]] | False |  |
| u | [[Character]] | True |  |
| user | [[Character]] | True |  |

## Script variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| CanPerform | [[Function]] | False |  |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[CombatEffect#^finish729994674\|Finish()]] | [[Void]] |  |  |
| [[CombatEffect#^scaleddamage1022549120\|ScaledDamage()]] | [[Damage]] | [[Character]] u |  |
| [[CombatEffect#^selecttargets1019762427\|SelectTargets()]] | [[Void]] | [[Targeting]] targeting, [[FunctionBase]] callback |  |
| [[CombatEffect#^waitforprojectiles-106052235\|WaitForProjectiles()]] | [[Void]] | [[FunctionBase]] callback |  |
| [[CombatEffect#^spawnprojectile49259087\|SpawnProjectile()]] | [[Projectile]] | [[GridItem]] target, [[String]] image, \[[[FunctionBase]] callback\] |  |
| [[CombatEffect#^spawnprojectile2010915657\|SpawnProjectile()]] | [[Projectile]] | [[Vector3D]] spawn, [[Vector3D]] target, [[String]] image, \[[[FunctionBase]] callback\] | |

## Script functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |



### Finish () : [[Void]]

^finish729994674

This is a function.

### ScaledDamage ([[Character]] u) : [[Damage]]

^scaleddamage1022549120

This is a function.

> [!Abstract]+ Parameters
> 1. `u` This is a parameter.

> [!Success]+ Return value
> Returns a [[Damage]].

### SelectTargets ([[Targeting]] targeting, [[FunctionBase]] callback) : [[Void]]

^selecttargets1019762427

This is a function.

> [!Abstract]+ Parameters
> 1. `targeting` This is a parameter.
> 2. `callback` This is a parameter.

### WaitForProjectiles ([[FunctionBase]] callback) : [[Void]]

^waitforprojectiles-106052235

This is a function.

> [!Abstract]+ Parameters
> 1. `callback` This is a parameter.

### SpawnProjectile ([[GridItem]] target, [[String]] image, \[[[FunctionBase]] callback\]) : [[Projectile]]

^spawnprojectile49259087

This is a function.

> [!Abstract]+ Parameters
> 1. `target` This is a parameter.
> 2. `image` This is a parameter.
> 3. `callback` This is a parameter.

> [!Success]+ Return value
> Returns a [[Projectile]].

### SpawnProjectile ([[Vector3D]] spawn, [[Vector3D]] target, [[String]] image, \[[[FunctionBase]] callback\]) : [[Projectile]]

^spawnprojectile2010915657

This is a function.

> [!Abstract]+ Parameters
> 1. `spawn` This is a parameter.
> 2. `target` This is a parameter.
> 3. `image` This is a parameter.
> 4. `callback` This is a parameter.

> [!Success]+ Return value
> Returns a [[Projectile]].

