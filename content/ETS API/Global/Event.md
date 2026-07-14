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
| [[Event#^raiseevent1805716478\|RaiseEvent()]] | [[Bool]] | [[EventData]] eventData | Announces an event to all listeners. |
| [[Event#^register1709452510\|Register()]] | [[Void]] | [[EventListener]] listener | Starts a listener watching for events. |
| [[Event#^remove-980187733\|Remove()]] | [[Void]] | [[EventListener]] listener | Stops a listener. |


### RaiseEvent ([[EventData]] eventData) : [[Bool]]

^raiseevent1805716478

Announces a game event to every listener, giving them a chance to react to it or to cancel it. Use it to fire your own custom events that other scripts can respond to.

> [!Abstract]+ Parameters
> 1. `eventData` The event to announce, carrying its details.

> [!Success]+ Return value
> Returns true if the event may go ahead, or false if a listener cancelled it.

### Register ([[EventListener]] listener) : [[Void]]

^register1709452510

Starts a listener watching for its event type, so it begins reacting when matching events happen.

> [!Example]+ Example
> Register a listener created for a combat summon:
> ```js
> Event.Register(listener);
> ```

> [!Abstract]+ Parameters
> 1. `listener` The listener to start.

### Remove ([[EventListener]] listener) : [[Void]]

^remove-980187733

Stops a listener, so it no longer reacts to events. Use it to clean up a listener you registered once it's no longer needed.

> [!Abstract]+ Parameters
> 1. `listener` The listener to stop.

