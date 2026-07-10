---
title: EventType
draft: false
tags:
 - ScriptType
 - ClassEnum
---
# EventType : [[ClassEnum]]

Some gameplay effects raise events when they occur. It is possible to listen for these types of events by creating an [[EventListener]], and running a triggered [[FunctionBase]] in response to them. An [[EventListener]] needs to be assigned a single [[EventType]] to listen for. When an event of the matching type is raised, the listener will trigger.

Example:
```js
var s = new StatusEffect(1);
s.name = "Stun";
s.description = "Unable to move and perform actions.";
s.image = "icon/skull.png";

var l = s.CreateListener("UnitStartTurn");
l.If = StunTrigger;
l.Do = StunEffect;

t.AddStatus(s);
```

> [!Hint]
> By using [[EventData#^stop1407120757|EventData.Stop()]] within [[EventListener#^23570a|EventListener.Do()]], it is possible to interrupt a raised event before it has time to happen. For most (but not all) event types, this will prevent the event from taking place.


## Enum values
| Id  | Name           | Description                                                                                                                                          |
| --- | -------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------- |
| 0 | Debug  |  |
| 1 | CombatStart  | Raised when a combat begins, before the first unit takes their turn. |
| 2 | CombatEnd  | Raised at the end of combat, before any rewards are presented. |
| 10 | UnitStartTurn  | Raised when any [[Character]] begins their turn. If stopped, the character won't get any actions or moves this turn. |
| 11 | UnitEndTurn  | Raised when any [[Character]] ends their turn. This is the same time that [[StatusEffect#^ontick\|StatusEffect.OnTick()]] happens for the character. |
| 12 | Movement  | Raised when any [[Character]] attempts to move. If interrupted, the character won't get to move. |
| 13 | Ability  | Raised when any [[Ability]] is used. If interrupted, the ability won't get performed, but the user still loses their action for the turn. |
| 14 | Attack  | Raised when any [[Character]] is about to perform an [[Attack]]. If interrupted, the attack will be prevented. |
| 15 | Damage  | Raised when any [[Character]] is about to be dealt [[Damage]]. If interrupted, the character will be treated as "Immune" and no damage is dealt. |
| 16 | Healing  | Raised when any [[Character]] is about to be dealt [[Damage]]. If interrupted, the character will not receive any healing. |
| 17 | ChangeStat  | Depricated and pending removal. |
| 18 | AddStatus  | Raised when any [[Character]] is about to have an [[Status]] applied to them. If interrupted, the effect won't be applied. |
| 19 | RemoveStatus  |  |
| 20 | AddTrait  |  |
| 21 | RemoveTrait  |  |
| 100 | ItemCanConsume  |  |
| 101 | ItemCanUse  |  |
| 102 | ItemCanEquip  |  |
| 103 | ItemCanUnequip  |  |
| 110 | ItemConsume  |  |
| 111 | ItemUse  |  |
| 112 | ItemEquip  |  |
| 113 | ItemUnequip  |  |


