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
| isUnique | [[Bool]] | True |  |
| duration | [[Int]] | False |  |
| value | [[Int]] | False |  |
| image | [[String]] | False |  |
| description | [[String]] | False |  |

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
| [[StatusEffect#^addtrait\|AddTrait()]] | [[Bool]] | [[TraitType]] trait |  |
| [[StatusEffect#^removetrait\|RemoveTrait()]] | [[Bool]] | [[TraitType]] trait |  |
| [[StatusEffect#^onapply\|OnApply()]] | [[Void]] | [[Character]] c |  |
| [[StatusEffect#^onremove\|OnRemove()]] | [[Void]] | [[Character]] c |  |
| [[StatusEffect#^ontick\|OnTick()]] | [[Void]] | [[Character]] c |  |

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

### OnApply ([[Character]] c) : [[Void]]

^onapply

Description goes here.

> [!Abstract]+ Parameters
> 1. `c` This is a parameter.

### OnRemove ([[Character]] c) : [[Void]]

^onremove

Description goes here.

> [!Abstract]+ Parameters
> 1. `c` This is a parameter.

### OnTick ([[Character]] c) : [[Void]]

^ontick

Description goes here.

> [!Abstract]+ Parameters
> 1. `c` This is a parameter.

