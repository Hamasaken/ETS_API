---
title: Sound
draft: false
tags:
 - Scope
---
# Sound

Can be used in any script through the global alias "Sound".

Example:
```js
// Play the sound of walking through bushes with a random pitch
Sound.PlaySound("sfx/bush1.wav", true);
```


## Script variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |


## Script functions
| Name                                                           | Return type | Parameters                                                          | Note |
| -------------------------------------------------------------- | ----------- | ------------------------------------------------------------------- | ---- |
| [[Sound#^stopmusic-246627812\|StopMusic()]] | [[Void]] |  | Stops the current music. |
| [[Sound#^changemusic1927404884\|ChangeMusic()]] | [[Void]] | [[String]] soundId | Switches to a new music track. |
| [[Sound#^stopambience-265757329\|StopAmbience()]] | [[Void]] |  | Stops the current ambient sound. |
| [[Sound#^changeambience1137557127\|ChangeAmbience()]] | [[Void]] | [[String]] soundId | Switches to a new ambient sound. |
| [[Sound#^playsound123292869\|PlaySound()]] | [[Void]] | [[String]] soundId, \[[[Bool]] randomPitch\] | Plays a one-off sound effect. |
| [[Sound#^playsoundat-1712376831\|PlaySoundAt()]] | [[Void]] | [[String]] soundId, [[Vector3D]] position, \[[[Bool]] randomPitch\] | Plays a sound effect at a world position. |


### StopMusic () : [[Void]]

^stopmusic-246627812

Stops whatever music is currently playing, leaving silence until a new track is started.

### ChangeMusic ([[String]] soundId) : [[Void]]

^changemusic1927404884

Switches the background music to a new track, replacing whatever was playing.

> [!Abstract]+ Parameters
> 1. `soundId` The id of the music track to play.

### StopAmbience () : [[Void]]

^stopambience-265757329

Stops the current ambient background sound (such as wind or waves).

### ChangeAmbience ([[String]] soundId) : [[Void]]

^changeambience1137557127

Switches the ambient background sound to a new one, replacing whatever was playing.

> [!Abstract]+ Parameters
> 1. `soundId` The id of the ambient sound to play.

### PlaySound ([[String]] soundId, \[[[Bool]] randomPitch\]) : [[Void]]

^playsound123292869

Plays a one-off sound effect, such as a footstep or a spell noise. Turn on random pitch to slightly vary the sound each time, so repeated plays don't sound identical.

> [!Example]+ Example
> Play a footstep sound with a slightly randomised pitch:
> ```js
> Sound.PlaySound("sfx/bush1.wav", true);
> ```

> [!Abstract]+ Parameters
> 1. `soundId` The id of the sound effect to play.
> 2. `randomPitch` True to vary the pitch slightly. Leave out to play it unchanged.

### PlaySoundAt ([[String]] soundId, [[Vector3D]] position, \[[[Bool]] randomPitch\]) : [[Void]]

^playsoundat-1712376831

Plays a sound effect at a particular spot in the 3D world, so it comes from that location — quieter and off to the side when it's far from the camera. Turn on random pitch to slightly vary the sound each time.

> [!Abstract]+ Parameters
> 1. `soundId` The id of the sound effect to play.
> 2. `position` Where in the world the sound comes from.
> 3. `randomPitch` True to vary the pitch slightly. Leave out to play it unchanged.

