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
| [[Asset#^spawnability1316364250\|SpawnAbility()]] | [[Ability]] | [[String]] id |  |
| [[Asset#^spawncharacter-148639875\|SpawnCharacter()]] | [[Character]] | [[String]] id |  |
| [[Asset#^spawnitem1488614075\|SpawnItem()]] | [[Item]] | [[String]] id |  |
| [[Asset#^spawnstatus638359384\|SpawnStatus()]] | [[Status]] | [[String]] id |  |


### SpawnAbility ([[String]] id) : [[Ability]]

^spawnability1316364250

This is a function.

> [!Abstract]+ Parameters
> 1. `id` This is a parameter.

> [!Success]+ Return value
> Returns a [[Ability]].

### SpawnCharacter ([[String]] id) : [[Character]]

^spawncharacter-148639875

This is a function.

> [!Abstract]+ Parameters
> 1. `id` This is a parameter.

> [!Success]+ Return value
> Returns a [[Character]].

### SpawnItem ([[String]] id) : [[Item]]

^spawnitem1488614075

This is a function.

> [!Abstract]+ Parameters
> 1. `id` This is a parameter.

> [!Success]+ Return value
> Returns a [[Item]].

### SpawnStatus ([[String]] id) : [[Status]]

^spawnstatus638359384

This is a function.

> [!Abstract]+ Parameters
> 1. `id` This is a parameter.

> [!Success]+ Return value
> Returns a [[Status]].

