---
title: TeamType
draft: false
tags:
 - ScriptType
 - ClassEnum
---
# TeamType : [[ClassEnum]]

Every unit on the battlefield needs to be assigned to a team. The teams represent the alignments of the units and keep track of who their allies/enemies are.

The "Player" team is reserved for the active player. "Team1", "Team2" and "Team3" represent enemy factions that are all hostile to the player. "Neutral" units count as both allies and enemies for all other teams when filtering ability targets and so on.

## Enum values
| Id  | Name    | Description                                                                          |
| --- | ------- | ------------------------------------------------------------------------------------ |
| 0 | Neutral  | Neutral with other teams, count as both allies and enemies to all. |
| 1 | Player  | These units typically belong to the player's party, or have joined them temporarily. |
| 2 | Team1  | Units from this team are hostile to all other teams. |
| 3 | Team2  | Units from this team are hostile to all other teams. |
| 4 | Team3  | Units from this team are hostile to all other teams. |




