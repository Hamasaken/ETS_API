---
title: Asset
draft: false
tags:
 - Scope
---
# Asset

The asset hooks are a set of functions for spawning and managing instances of assets.

Can be used in any script through the global alias "Asset".

Example:
```js
var c = Asset.SpawnCharacter("bob");
var itm = Asset.SpawnItem("fun_bomb");
```


## Script variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |


## Script functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Asset#^spawnability1316364250\|SpawnAbility()]] | [[Ability]] | [[String]] id | Creates a fresh ability from its id. |
| [[Asset#^spawncharacter-148639875\|SpawnCharacter()]] | [[Character]] | [[String]] id | Creates a fresh character from its id. |
| [[Asset#^spawnitem1488614075\|SpawnItem()]] | [[Item]] | [[String]] id | Creates a fresh item from its id. |
| [[Asset#^spawnstatus638359384\|SpawnStatus()]] | [[Status]] | [[String]] id | Creates a fresh status from its id. |


### SpawnAbility ([[String]] id) : [[Ability]]

^spawnability1316364250

Creates a fresh copy of an [[Ability]] from its id, ready to be given to a character or performed.

> [!Abstract]+ Parameters
> 1. `id` The id of the ability to create.

> [!Success]+ Return value
> Returns the newly created ability.

### SpawnCharacter ([[String]] id) : [[Character]]

^spawncharacter-148639875

Creates a fresh copy of a [[Character]] from its id — for example a summoned creature to bring into a fight.

> [!Example]+ Example
> Create a character, then place it into combat:
> ```js
> var c = Asset.SpawnCharacter("bob");
> ```

> [!Abstract]+ Parameters
> 1. `id` The id of the character to create.

> [!Success]+ Return value
> Returns the newly created character.

### SpawnItem ([[String]] id) : [[Item]]

^spawnitem1488614075

Creates a fresh copy of an [[Item]] from its id, ready to be placed in an inventory or used.

> [!Abstract]+ Parameters
> 1. `id` The id of the item to create.

> [!Success]+ Return value
> Returns the newly created item.

### SpawnStatus ([[String]] id) : [[Status]]

^spawnstatus638359384

Creates a fresh copy of a [[Status]] effect from its id, ready to be applied to a character.

> [!Abstract]+ Parameters
> 1. `id` The id of the status to create.

> [!Success]+ Return value
> Returns the newly created status.

