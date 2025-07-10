---
title: AssetHooks
draft: false
tags:
 - ScriptObject
---

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

Description goes here.

> [!Abstract]+ Parameters
> 1. `id` This is a parameter.

> [!Success]+ Return value
> Returns a [[Ability]].

### SpawnCharacter ([[String]] id) : [[Character]]

^spawncharacter

Description goes here.

> [!Abstract]+ Parameters
> 1. `id` This is a parameter.

> [!Success]+ Return value
> Returns a [[Character]].

### SpawnItem ([[String]] id) : [[Item]]

^spawnitem

Description goes here.

> [!Abstract]+ Parameters
> 1. `id` This is a parameter.

> [!Success]+ Return value
> Returns a [[Item]].

### SpawnStatus ([[String]] id) : [[Status]]

^spawnstatus

Description goes here.

> [!Abstract]+ Parameters
> 1. `id` This is a parameter.

> [!Success]+ Return value
> Returns a [[StatusEffect]].

