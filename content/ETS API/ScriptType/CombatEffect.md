---
title: CombatEffect
draft: false
tags:
 - ScriptType
 - ScriptObject
---
# CombatEffect : [[Any]]

A CombatEffect is one step of what an [[Ability]] or [[Item]] does in battle — pick targets, fire a projectile, deal damage, apply a status. It carries the [[Targeting]] rules, an optional [[Attack]] and [[Damage]], and a [[StatScaling]], and its script drives the sequence: choosing targets, spawning projectiles, and finishing up. An ability or item runs its combat effects one after another.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| targeting | [[Targeting]] | False | The rules for which tiles or units this effect can target. |
| attack | [[Attack]] | False | The attack used to roll for hits, if any. |
| damage | [[Damage]] | False | The base damage this effect deals, if any. |
| scaling | [[StatScaling]] | False | How the damage grows with one of the user's stats. |
| u | [[Character]] | True | The character performing the effect (shorthand for `user`). |
| user | [[Character]] | True | The character performing the effect. |

## Script variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| CanPerform | [[Function]] | False | Your check for whether the effect can be carried out. |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[CombatEffect#^finish729994674\|Finish()]] | [[Void]] |  | Signals this effect is done. |
| [[CombatEffect#^scaleddamage1022549120\|ScaledDamage()]] | [[Damage]] | [[Character]] u | The damage after stat scaling is added. |
| [[CombatEffect#^selecttargets1019762427\|SelectTargets()]] | [[Void]] | [[Targeting]] targeting, [[FunctionBase]] callback | Choose targets, then run a callback. |
| [[CombatEffect#^waitforprojectiles-106052235\|WaitForProjectiles()]] | [[Void]] | [[FunctionBase]] callback | Wait for projectiles to land, then run a callback. |
| [[CombatEffect#^spawnprojectile49259087\|SpawnProjectile()]] | [[Projectile]] | [[GridItem]] target, [[String]] image, \[[[FunctionBase]] callback\] | Launch a projectile at a target. |
| [[CombatEffect#^spawnprojectile2010915657\|SpawnProjectile()]] | [[Projectile]] | [[Vector3D]] spawn, [[Vector3D]] target, [[String]] image, \[[[FunctionBase]] callback\] | Launch a projectile between two points. |

## Script functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |



### Finish () : [[Void]]

^finish729994674

Signals that this combat effect is done, letting the ability or item move on to its next step. Usually called once all targets have been resolved and any projectiles have landed.

> [!Example]+ Example
> Finish the effect once every projectile has hit:
> ```js
> WaitForProjectiles(() => Finish());
> ```

### ScaledDamage ([[Character]] u) : [[Damage]]

^scaleddamage1022549120

Gives the effect's [[Damage]] with its stat scaling added in for the given character — the actual amount to deal. If the effect has no scaling, this is just its base damage.

> [!Example]+ Example
> Deal the effect's scaled damage to a character that was hit:
> ```js
> c.TakeDamage(ScaledDamage(u));
> ```

> [!Abstract]+ Parameters
> 1. `u` The character whose stat drives the scaling — usually the user.

> [!Success]+ Return value
> Returns the final damage after scaling.

### SelectTargets ([[Targeting]] targeting, [[FunctionBase]] callback) : [[Void]]

^selecttargets1019762427

Asks the player (or the AI) to choose targets according to the given [[Targeting]] rules, then runs your callback with the chosen targets once they are picked. This is usually the first step of a combat effect's script.

> [!Example]+ Example
> Pick targets and continue in an `OnTargets` function:
> ```js
> SelectTargets(targeting, OnTargets);
> ```

> [!Abstract]+ Parameters
> 1. `targeting` The rules deciding what can be targeted.
> 2. `callback` A function that runs once targets are chosen, receiving the result.

### WaitForProjectiles ([[FunctionBase]] callback) : [[Void]]

^waitforprojectiles-106052235

Waits until every projectile this effect has spawned has landed, then runs your callback. This lets the script hold off finishing until the on-screen projectiles catch up.

> [!Example]+ Example
> Finish the effect only after all projectiles hit:
> ```js
> WaitForProjectiles(() => Finish());
> ```

> [!Abstract]+ Parameters
> 1. `callback` A function that runs once all projectiles have landed.

### SpawnProjectile ([[GridItem]] target, [[String]] image, \[[[FunctionBase]] callback\]) : [[Projectile]]

^spawnprojectile49259087

Launches a projectile from the user toward a target tile or unit, showing the given image, and optionally runs a callback when it lands. It returns the [[Projectile]] so you can decorate it further, for example by adding a trail.

> [!Example]+ Example
> Fire a projectile at a target and react when it hits:
> ```js
> var p = SpawnProjectile(t, projectileImage, OnProj).AddTrail(projectileTrail);
> ```

> [!Abstract]+ Parameters
> 1. `target` The tile or unit to fire at.
> 2. `image` The picture to use for the projectile.
> 3. `callback` A function that runs when the projectile lands. Optional.

> [!Success]+ Return value
> Returns the spawned projectile.

### SpawnProjectile ([[Vector3D]] spawn, [[Vector3D]] target, [[String]] image, \[[[FunctionBase]] callback\]) : [[Projectile]]

^spawnprojectile2010915657

The same as the other [[CombatEffect#^spawnprojectile49259087\|SpawnProjectile()]], but you give explicit start and end positions in the 3D world instead of firing at a target on the grid. Use this when you need precise control over where the projectile travels.

> [!Abstract]+ Parameters
> 1. `spawn` The position the projectile starts from.
> 2. `target` The position the projectile flies to.
> 3. `image` The picture to use for the projectile.
> 4. `callback` A function that runs when the projectile lands. Optional.

> [!Success]+ Return value
> Returns the spawned projectile.

