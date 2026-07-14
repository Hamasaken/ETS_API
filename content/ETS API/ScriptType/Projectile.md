---
title: Projectile
draft: false
tags:
 - ScriptType
---
# Projectile : [[Any]]

A Projectile is a moving visual fired between two points in combat — an arrow, a bolt, a thrown flask. A [[CombatEffect]] spawns one with [[CombatEffect#^spawnprojectile49259087\|SpawnProjectile()]] and can decorate it, for example by adding a trail, before it flies to its target.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| speed | [[Float]] | False | How fast the projectile travels. |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Projectile#^addtrail1792537319\|AddTrail()]] | [[Projectile]] | [[Int]] id | Adds a visual trail behind the projectile. |



### AddTrail ([[Int]] id) : [[Projectile]]

^addtrail1792537319

Adds a visual trail effect behind the projectile, chosen by its id. It returns the same projectile, so you can chain it straight onto a spawn call.

> [!Example]+ Example
> Fire a projectile and give it a trail in one line:
> ```js
> var p = SpawnProjectile(t, projectileImage, OnProj).AddTrail(projectileTrail);
> ```

> [!Abstract]+ Parameters
> 1. `id` The id of the trail effect to add.

> [!Success]+ Return value
> Returns the same projectile, so further changes can be chained.

