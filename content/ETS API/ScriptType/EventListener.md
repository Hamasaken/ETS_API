---
title: EventListener
draft: false
tags:
 - ScriptType
 - ScriptObject
---
# EventListener : [[Any]]

An EventListener watches for a particular kind of game event (its [[EventType]]) and reacts when one happens. Its `If` script decides whether a given occurrence is relevant, and its `Do` script carries out the response. Traits, statuses and items add listeners to change how the game behaves; when several are watching the same event, higher-priority ones react first.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| type | [[EventType]] | True | Which kind of event this listener reacts to. |
| priority | [[Int]] | False | Run order; higher priority reacts first. |

## Script variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| If | [[Function]] | False | Your check for whether to respond to this event. |
| Do | [[Function]] | False | Your response, run when the If check passes. |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Script functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |



