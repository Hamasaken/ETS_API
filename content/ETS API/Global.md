---
title: Global
draft: false
tags:
 - Scope
---
# Global

Every script always has access to the variables and functions in the global scope. Most of the variables in here are different hooks for gameplay managers.

Be aware that these members can be hidden if the same names are used by other [[ScriptType|ScriptTypes]] and [[Scope|Scopes]] for their own members.

## Script variables
| Name          | Type      | Readonly | Note |
| ------------- | --------- | -------- | ---- |
| [[Asset]] | [[Scope]] | True | Spawn fresh characters, items, abilities and statuses. |
| [[Adventure]] | [[Scope]] | True | The overworld journey, party and inventory. |
| A | [[Scope]] | True | Shorthand alias for [[Adventure]]. |
| [[Combat]] | [[Scope]] | True | The current fight — units, the map and turns. |
| C | [[Scope]] | True | Shorthand alias for [[Combat]]. |
| [[Event]] | [[Scope]] | True | Raise game events and register listeners. |
| E | [[Scope]] | True | Shorthand alias for [[Event]]. |
| [[Sound]] | [[Scope]] | True | Play music, ambience and sound effects. |
| S | [[Scope]] | True | Shorthand alias for [[Sound]]. |
| [[Math]] | [[Scope]] | True | Number helpers — rounding, min/max, powers and more. |
| [[Random]] | [[Scope]] | True | Random numbers for chances and rolls. |


## Script functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |


