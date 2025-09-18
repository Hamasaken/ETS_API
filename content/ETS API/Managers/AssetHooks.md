---
title: AssetHooks
draft: false
tags:
 - ScriptObject
---

The asset hooks are a set of functions for spawning and managing instances of assets.

Can be used in any script through the global alias "Asset".

Example:
```js
var c = Asset.SpawnCharacter("bob");
var itm = Asset.SpawnItem("fun_bomb");
```


## Variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[AssetHooks#^spawnability\|SpawnAbility()]] | [[Ability]] | [[String]] id |  |
| [[AssetHooks#^spawncharacter\|SpawnCharacter()]] | [[Character]] | [[String]] id |  |
| [[AssetHooks#^spawnitem\|SpawnItem()]] | [[Item]] | [[String]] id |  |
| [[AssetHooks#^spawnstatus\|SpawnStatus()]] | [[Status]] | [[String]] id |  |

### SpawnAbility ([[String]] id) : [[Ability]]

^spawnability

Creates a new instance of an ability asset.

> [!Abstract]+ Parameters
> 1. `id` The id of the ability to spawn.

> [!Success]+ Return value
> Returns the newly created [[Ability]] instance.

### SpawnCharacter ([[String]] id) : [[Character]]

^spawncharacter

Creates a new instance of a character asset.

> [!Abstract]+ Parameters
> 1. `id` The id of the character to spawn.

> [!Success]+ Return value
> Returns the newly created [[Character]] instance.

### SpawnItem ([[String]] id) : [[Item]]

^spawnitem

Creates a new instance of an item asset.

> [!Abstract]+ Parameters
> 1. `id` The id of the item to spawn.

> [!Success]+ Return value
> Returns the newly created [[Item]] instance.

### SpawnStatus ([[String]] id) : [[Status]]

^spawnstatus

Creates a new instance of a status asset.

> [!Abstract]+ Parameters
> 1. `id` The id of the status to spawn.

> [!Success]+ Return value
> Returns the newly created [[Status]] instance.

