---
title: Damage
draft: false
tags:
 - ScriptType
---
# Damage : [[Any]]

A Damage bundles up a hit dealt to a [[Character]]: how much (`value`), what kind (`type`, such as Fire or Physical), and whether it ignores armour (`pen`). Effects build a Damage and deal it with [[Character#^takedamage-638525238\|TakeDamage()]]; unless it penetrates, the character's Defense reduces it first.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| type | [[DamageType]] | False | The kind of damage (Physical, Fire, Frost…). |
| value | [[Int]] | False | How much damage this deals (never below 0). |
| pen | [[Bool]] | False | When true, ignores the target's Defense. |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |



