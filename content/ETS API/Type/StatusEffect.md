---
title: StatusEffect
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
| duration | [[Int]] | False |  |
| value | [[Int]] | False |  |
| OnRemove | [[Void]] | False |  |
| OnTick | [[Void]] | False |  |

^709a4f


## Functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[StatusEffect#^createlistener\|CreateListener()]] | [[EventListener]] | [[EventType]] event, [[Int]] priority |  |
| [[StatusEffect#^addlistener\|AddListener()]] | [[Void]] | [[EventListener]] listener |  |
| [[StatusEffect#^removelistener\|RemoveListener()]] | [[Void]] | [[EventListener]] listener |  |
| [[StatusEffect#^clearlisteners\|ClearListeners()]] | [[Void]] |  |  |
| [[StatusEffect#^istrait\|IsTrait()]] | [[Bool]] | [[TraitType]] trait |  |
| [[StatusEffect#^hastrait\|HasTrait()]] | [[Bool]] | [[TraitType]] trait |  |
| [[StatusEffect#^addtrait\|AddTrait()]] | [[Void]] | [[TraitType]] trait |  |
| [[StatusEffect#^onapply\|OnApply()]] | [[Void]] | [[Character]] c |  |

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

### AddTrait ([[TraitType]] trait) : [[Void]]

^addtrait

Description goes here.

> [!Abstract]+ Parameters
> 1. `trait` This is a parameter.

### OnApply ([[Character]] c) : [[Void]]

^onapply

Description goes here.

> [!Abstract]+ Parameters
> 1. `c` This is a parameter.

