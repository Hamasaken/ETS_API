---
title: EventManager
draft: false
tags:
 - ScriptObject
---

Can be used in any script through the global alias "Event".

Example:
```js
// Code for a summon in combat
var listener = new EventListener("UnitStartTurn", 100);
Event.Register(listener);
```


## Variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[EventManager#^raiseevent\|RaiseEvent()]] | [[Bool]] | [[EEvent]] eventData | |
| [[EventManager#^register\|Register()]] | [[Void]] | [[EventListener]] listener | |
| [[EventManager#^remove\|Remove()]] | [[Void]] | [[EventListener]] listener | |

### RaiseEvent ([[EEvent]] eventData) : [[Bool]]

^raiseevent

Description goes here.

> [!Abstract]+ Parameters
> 1. `eventData` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### Register ([[EventListener]] listener) : [[Void]]

^register

Description goes here.

> [!Abstract]+ Parameters
> 1. `listener` This is a parameter.

### Remove ([[EventListener]] listener) : [[Void]]

^remove

Description goes here.

> [!Abstract]+ Parameters
> 1. `listener` This is a parameter.

