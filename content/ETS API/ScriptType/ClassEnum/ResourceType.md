---
title: ResourceType
draft: false
tags:
 - ScriptType
 - ClassEnum
---
# ResourceType : [[ClassEnum]]

A ResourceType describes a kind of [[Resource]] pool and how it behaves: where its maximum comes from (a backing [[Stat]], possibly scaled, or a fixed number), whether the current amount follows the maximum when that stat changes, whether the pool starts full or empty, and what colors its bar is drawn with. Health and Mana are built in and every character has them; new types can be added in the `.resources` asset file without touching code.

## Enum values
| Id     | Name    | Maximum          | Scales with max | Colors           | Description |
| ------ | ------- | ---------------- | --------------- | ---------------- | ----------- |
| 0 | Health | Health * 1 | True | 74140B, 74140B  | The character's life; emptying it kills them. |
| 1 | Mana | Mana * 1 | True | 192C5B, 192C5B  | Spent to power abilities. |
| 9999 | Debug | Debug * 1 | True |   | For testing only. |
| 100000 | Stamina | Constitution * 2 | True |   | Defined in the `.resources` asset file; caps at twice Constitution. |
| 100001 | Shield | 30 | True |   | Defined in the `.resources` asset file; fixed cap of 30, starts empty. |


