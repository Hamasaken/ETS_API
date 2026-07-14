---
title: EventData
draft: false
tags:
 - ScriptType
 - ScriptObject
---
# EventData : [[Any]]

An EventData carries the details of a single game event as it happens — what kind it is, and the things involved (the character, target, damage, item, and so on). Event listeners read these details to decide how to react, and can change them before the event resolves. Calling [[EventData#^stop-1406502445\|Stop()]] cancels the event.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| type | [[EventType]] | True | Which kind of event this is. |
| stopped | [[Bool]] | True | True once the event has been cancelled. |

## Script variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[EventData#^stop-1406502445\|Stop()]] | [[Void]] |  | Cancels the event. |

## Script functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |



### Stop () : [[Void]]

^stop-1406502445

Cancels the event so it does not go ahead. Listeners use this to block something from happening — for example, preventing a hit from dealing its damage.

