---
title: UnitVisuals
draft: false
tags:
 - ScriptType
---
# UnitVisuals : [[CharacterVisuals]]

UnitVisuals is a [[Unit]]'s on-screen representation on the combat grid. It can do everything [[CharacterVisuals]] can — play animations and show floating text — plus grid-specific things: facing a direction, and reporting its position in the 3D world. Combat scripts use it to drive a unit's animations and floating text.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[UnitVisuals#^getcenterposition-706170835\|GetCenterPosition()]] | [[Vector3D]] |  | The unit's centre position in the 3D world. |
| [[UnitVisuals#^getposition508150146\|GetPosition()]] | [[Vector3D]] |  | The unit's position in the 3D world. |
| [[UnitVisuals#^facetowards763389658\|FaceTowards()]] | [[Void]] | [[GridItem]] position | Turns the unit to face a position. |
| [[UnitVisuals#^floatingtext-749008862\|FloatingText()]] | [[Void]] | [[String]] text | Pops a short piece of text above the unit. |
| [[UnitVisuals#^floatingtext-1744420634\|FloatingText()]] | [[Void]] | [[String]] text, [[String]] style | Pops text above the unit in a given style. |
| [[UnitVisuals#^playanimation109847255\|PlayAnimation()]] | [[Void]] | [[String]] animation | Plays a named animation on the unit. |
| [[UnitVisuals#^playanimation-889683853\|PlayAnimation()]] | [[Void]] | [[String]] animation, [[FunctionBase]] callback | Plays an animation, then runs a callback. |
| [[UnitVisuals#^addevent1387404664\|AddEvent()]] | [[Void]] | [[FunctionBase]] callback | Runs a function at the animation's event moment. |
| [[UnitVisuals#^setend1118996200\|SetEnd()]] | [[Void]] | [[FunctionBase]] callback | Runs a function when the animation finishes. |



### GetCenterPosition () : [[Vector3D]]

^getcenterposition-706170835

Gives the position at the middle of the unit in the 3D world — handy as a start or end point for projectiles so they aim at the body rather than the feet.

> [!Success]+ Return value
> Returns the unit's centre position in the world.

### GetPosition () : [[Vector3D]]

^getposition508150146

Gives the unit's position in the 3D world, at its base on the ground.

> [!Success]+ Return value
> Returns the unit's position in the world.

### FaceTowards ([[GridItem]] position) : [[Void]]

^facetowards763389658

Turns the unit so it faces toward a grid position — for example to look at its target before attacking.

> [!Abstract]+ Parameters
> 1. `position` The grid position to face toward.

### FloatingText ([[String]] text) : [[Void]]

^floatingtext-749008862

Pops a short piece of text into the air above the unit, such as a damage number or a word like "Blocked" or "Missed".

> [!Example]+ Example
> Show a burst of text above the unit:
> ```js
> c.visuals.FloatingText('*BOOOM!*')
> ```

> [!Abstract]+ Parameters
> 1. `text` The text to show above the unit.

### FloatingText ([[String]] text, [[String]] style) : [[Void]]

^floatingtext-1744420634

The same as the plain [[UnitVisuals#^floatingtext-749008862\|FloatingText()]], but shown with a particular visual style — useful to make, say, healing look different from damage.

> [!Abstract]+ Parameters
> 1. `text` The text to show above the unit.
> 2. `style` The visual style to show it in.

### PlayAnimation ([[String]] animation) : [[Void]]

^playanimation109847255

Plays a named animation on the unit, such as an attack or a hurt reaction.

> [!Example]+ Example
> Play the hurt animation when a unit is damaged:
> ```js
> c.visuals.PlayAnimation("Hurt01")
> ```

> [!Abstract]+ Parameters
> 1. `animation` The name of the animation to play.

### PlayAnimation ([[String]] animation, [[FunctionBase]] callback) : [[Void]]

^playanimation-889683853

Plays a named animation and runs your callback once it finishes — handy for waiting until an attack animation completes before dealing its effect.

> [!Abstract]+ Parameters
> 1. `animation` The name of the animation to play.
> 2. `callback` A function to run once the animation finishes.

### AddEvent ([[FunctionBase]] callback) : [[Void]]

^addevent1387404664

Adds a function to run at the animation's event moment — a point marked partway through, such as the instant a strike is meant to land.

> [!Abstract]+ Parameters
> 1. `callback` A function to run at the animation's event moment.

### SetEnd ([[FunctionBase]] callback) : [[Void]]

^setend1118996200

Sets a function to run when the current animation finishes.

> [!Abstract]+ Parameters
> 1. `callback` A function to run once the animation ends.

