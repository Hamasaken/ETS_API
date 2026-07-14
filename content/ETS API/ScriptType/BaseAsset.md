---
title: BaseAsset
draft: false
tags:
 - ScriptType
---
# BaseAsset : [[Any]]

BaseAsset is the shared foundation for the game's loadable content — [[Character]]s, [[Item]]s, [[Status]] effects, [[TileMap]]s and more all build on it. It gives every asset an identity: an `id` shared by all copies of that content, a `uid` unique to one copy, and a `name` shown to the player.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| id | [[String]] | True | The content's id, shared by every copy of it. |
| uid | [[String]] | True | A unique id for this particular copy. |
| name | [[String]] | False | The name shown to the player. |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |



