---
title: EventAware
draft: false
tags:
 - ScriptType
---
# EventAware : [[Any]]

EventAware is the shared base for things that can register [[EventListener]]s — [[Character]]s, [[Item]]s, [[Status]] effects and [[Trait]]s all build on it. It lets them hook into game events while active and cleanly stop listening when they are removed.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[EventAware#^createlistener24257249\|CreateListener()]] | [[EventListener]] | [[EventType]] event, \[[[Int]] priority\] | Creates and registers a new listener. |
| [[EventAware#^addlistener-534891004\|AddListener()]] | [[Void]] | [[EventListener]] listener | Starts using a listener you built. |
| [[EventAware#^removelistener-1284705417\|RemoveListener()]] | [[Void]] | [[EventListener]] listener | Stops using a single listener. |
| [[EventAware#^clearlisteners-689026739\|ClearListeners()]] | [[Void]] |  | Removes all of its listeners at once. |



### CreateListener ([[EventType]] event, \[[[Int]] priority\]) : [[EventListener]]

^createlistener24257249

Creates a new [[EventListener]] for the given event type, registers it, and hands it back so you can fill in its `If` and `Do` scripts. Optionally set a priority to control when it runs relative to other listeners.

> [!Abstract]+ Parameters
> 1. `event` The kind of event to listen for.
> 2. `priority` Run order among listeners; higher reacts first. Leave out for the default.

> [!Success]+ Return value
> Returns the newly created listener.

### AddListener ([[EventListener]] listener) : [[Void]]

^addlistener-534891004

Starts using a listener you built yourself, registering it so it begins reacting to events.

> [!Abstract]+ Parameters
> 1. `listener` The listener to start using.

### RemoveListener ([[EventListener]] listener) : [[Void]]

^removelistener-1284705417

Stops using a single listener, so it no longer reacts to events.

> [!Abstract]+ Parameters
> 1. `listener` The listener to stop using.

### ClearListeners () : [[Void]]

^clearlisteners-689026739

Removes all of this thing's listeners at once, so none of them react to events any more. Usually done when it is removed from play.

