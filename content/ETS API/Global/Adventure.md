---
title: Adventure
draft: false
tags:
 - Scope
---
# Adventure

The adventure manager is responsible for keeping track of everything related to a playthrough of the game. Characters and items, quests, maps, and so on.

Can be used in any script through the global alias "Adventure" or "A".

Example:
```js
var c = Asset.SpawnCharacter("bob");
Adventure.party.Add(c);
```


## Script variables
| Name  | Type                    | Readonly | Note                                                                                                                                                         |
| ----- | ----------------------- | -------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| party | [[List]]<[[Character]]> | True | This is a [[List]] of the characters currently belonging to the player's party. Adding a character to the list will make them show up in events and combats. |
| inv | [[List]]<[[Item]]> | True | This is a [[List]] of the [[Item\|items]] the party is carrying along with them. |


## Script functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |


