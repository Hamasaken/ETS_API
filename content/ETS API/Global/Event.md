---
title: Event
draft: false
tags:
 - Scope
---
# Event

Can be used in any script through the global alias "Event".

Example:
```js
// Code for a summon in combat
var listener = new EventListener("UnitStartTurn", 100);
Event.Register(listener);
```


## Script variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |


## Script functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Event#^raiseevent1805716478\|RaiseEvent()]] | [[Bool]] | [[EventData]] eventData |  |
| [[Event#^register1709452510\|Register()]] | [[Void]] | [[EventListener]] listener |  |
| [[Event#^remove-980187733\|Remove()]] | [[Void]] | [[EventListener]] listener |  |


### RaiseEvent ([[EventData]] eventData) : [[Bool]]

^raiseevent1805716478

This is a function.

> [!Abstract]+ Parameters
> 1. `eventData` This is a parameter.

> [!Success]+ Return value
> Returns a [[Bool]].

### Register ([[EventListener]] listener) : [[Void]]

^register1709452510

This is a function.

> [!Abstract]+ Parameters
> 1. `listener` This is a parameter.

### Remove ([[EventListener]] listener) : [[Void]]

^remove-980187733

This is a function.

> [!Abstract]+ Parameters
> 1. `listener` This is a parameter.

