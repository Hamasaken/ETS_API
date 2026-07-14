---
title: FlagType
draft: false
tags:
 - ScriptType
 - ClassEnum
---
# FlagType : [[ClassEnum]]

Flags is a character specific field that tracks [[Bool]] values.

We recommend not messing with flags for now, since they might be changed in the near future.


## Enum values
| Id     | Name             | Description |
| ------ | ---------------- | ----------- |
| 0 | Default  | A catch-all default flag. |
| 1 | Alive  | Set while the character is alive; cleared when health reaches 0. |
| 2 | PlayerControlled  | Set when the player controls this character. |
| 3 | Ranged  | Marks the character as a ranged fighter. |
| 10 | Flying  | The character flies, ignoring most ground movement costs. |
| 100000 | Swimming  | The character can move through water. |
| 100001 | Restrained  | The character is held in place and cannot move. |


