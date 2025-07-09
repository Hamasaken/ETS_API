---
title: Item
draft: false
tags:
 - ScriptObject
---

Description goes here.

## Variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| id | [[String]] | False |  |
| name | [[String]] | False |  |
| image | [[String]] | False |  |
| description | [[String]] | False |  |
| consumeHint | [[String]] | False |  |
| useHint | [[String]] | False |  |
| equipHint | [[String]] | False |  |

## Functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Item#^createlistener\|CreateListener()]] | [[EventListener]] | [[EventType]] event, [[Int]] priority |  |
| [[Item#^addlistener\|AddListener()]] | [[Void]] | [[EventListener]] listener |  |
| [[Item#^removelistener\|RemoveListener()]] | [[Void]] | [[EventListener]] listener |  |
| [[Item#^clearlisteners\|ClearListeners()]] | [[Void]] |  |  |
| [[Item#^istrait\|IsTrait()]] | [[Bool]] | [[TraitType]] trait |  |
| [[Item#^hastrait\|HasTrait()]] | [[Bool]] | [[TraitType]] trait |  |
| [[Item#^addtrait\|AddTrait()]] | [[Bool]] | [[TraitType]] trait |  |
| [[Item#^removetrait\|RemoveTrait()]] | [[Bool]] | [[TraitType]] trait |  |
| [[Item#^finish\|Finish()]] | [[Void]] |  |  |
| [[Item#^canconsume\|CanConsume()]] | [[Bool]] | [[Character]] c |  |
| [[Item#^canuse\|CanUse()]] | [[Bool]] | [[Character]] c |  |
| [[Item#^canequip\|CanEquip()]] | [[Bool]] | [[Character]] c |  |
| [[Item#^canunequip\|CanUnequip()]] | [[Bool]] | [[Character]] c |  |
| [[Item#^onconsume\|OnConsume()]] | [[Void]] | [[Character]] c |  |
| [[Item#^onuse\|OnUse()]] | [[Void]] | [[Character]] c |  |
| [[Item#^onequip\|OnEquip()]] | [[Void]] | [[Character]] c |  |
| [[Item#^onunequip\|OnUnequip()]] | [[Void]] | [[Character]] c |  |

### CreateListener ([[EventType]] event, [[Int]] priority) : [[EventListener]]

^createlistener

Description goes here.

> [!Abstract]+ Parameters
> 1. `event` This is a parameter.
> 2. `priority` This is a parameter.

> [!Success]+ Return value
> Returns a [[EventListener]].

### AddListener ([[EventListener]] listener) : [[Void]]

^addlistener

Description goes here.

> [!Abstract]+ Parameters
> 1. `listener` This is a parameter.

### RemoveListener ([[EventListener]] listener) : [[Void]]

^removelistener

Description goes here.

> [!Abstract]+ Parameters
> 1. `listener` This is a parameter.

### ClearListeners () : [[Void]]

^clearlisteners

Description goes here.

### IsTrait ([[TraitType]] trait) : [[Bool]]

^istrait

Description goes here.

> [!Abstract]+ Parameters
> 1. `trait` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### HasTrait ([[TraitType]] trait) : [[Bool]]

^hastrait

Description goes here.

> [!Abstract]+ Parameters
> 1. `trait` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### AddTrait ([[TraitType]] trait) : [[Bool]]

^addtrait

Description goes here.

> [!Abstract]+ Parameters
> 1. `trait` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### RemoveTrait ([[TraitType]] trait) : [[Bool]]

^removetrait

Description goes here.

> [!Abstract]+ Parameters
> 1. `trait` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### Finish () : [[Void]]

^finish

Description goes here.

### CanConsume ([[Character]] c) : [[Bool]]

^canconsume

Description goes here.

> [!Abstract]+ Parameters
> 1. `c` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### CanUse ([[Character]] c) : [[Bool]]

^canuse

Description goes here.

> [!Abstract]+ Parameters
> 1. `c` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### CanEquip ([[Character]] c) : [[Bool]]

^canequip

Description goes here.

> [!Abstract]+ Parameters
> 1. `c` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### CanUnequip ([[Character]] c) : [[Bool]]

^canunequip

Description goes here.

> [!Abstract]+ Parameters
> 1. `c` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### OnConsume ([[Character]] c) : [[Void]]

^onconsume

Description goes here.

> [!Abstract]+ Parameters
> 1. `c` This is a parameter.

### OnUse ([[Character]] c) : [[Void]]

^onuse

Description goes here.

> [!Abstract]+ Parameters
> 1. `c` This is a parameter.

### OnEquip ([[Character]] c) : [[Void]]

^onequip

Description goes here.

> [!Abstract]+ Parameters
> 1. `c` This is a parameter.

### OnUnequip ([[Character]] c) : [[Void]]

^onunequip

Description goes here.

> [!Abstract]+ Parameters
> 1. `c` This is a parameter.

