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
| [[Sound#^stopmusic-246627812\|StopMusic()]] | [[Void]] |  |  |
| [[Sound#^changemusic1927404884\|ChangeMusic()]] | [[Void]] | [[String]] soundId |  |
| [[Sound#^stopambience-265757329\|StopAmbience()]] | [[Void]] |  |  |
| [[Sound#^changeambience1137557127\|ChangeAmbience()]] | [[Void]] | [[String]] soundId |  |
| [[Sound#^playsound123292869\|PlaySound()]] | [[Void]] | [[String]] soundId, \[[[Bool]] randomPitch\] |  |
| [[Sound#^playsoundat-1712376831\|PlaySoundAt()]] | [[Void]] | [[String]] soundId, [[Vector3D]] position, \[[[Bool]] randomPitch\] |  |


### StopMusic () : [[Void]]

^stopmusic-246627812

This is a function.

### ChangeMusic ([[String]] soundId) : [[Void]]

^changemusic1927404884

This is a function.

> [!Abstract]+ Parameters
> 1. `soundId` This is a parameter.

### StopAmbience () : [[Void]]

^stopambience-265757329

This is a function.

### ChangeAmbience ([[String]] soundId) : [[Void]]

^changeambience1137557127

This is a function.

> [!Abstract]+ Parameters
> 1. `soundId` This is a parameter.

### PlaySound ([[String]] soundId, \[[[Bool]] randomPitch\]) : [[Void]]

^playsound123292869

This is a function.

> [!Abstract]+ Parameters
> 1. `soundId` This is a parameter.
> 2. `randomPitch` This is a parameter.

### PlaySoundAt ([[String]] soundId, [[Vector3D]] position, \[[[Bool]] randomPitch\]) : [[Void]]

^playsoundat-1712376831

This is a function.

> [!Abstract]+ Parameters
> 1. `soundId` This is a parameter.
> 2. `position` This is a parameter.
> 3. `randomPitch` This is a parameter.

