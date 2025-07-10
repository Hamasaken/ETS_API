---
title: AdventureManager
draft: false
tags:
 - ScriptObject
---

Can be used in any script through the global alias "Adventure".

Example:
```js
var c = Asset.SpawnCharacter("bob");
Adventure.party.Add(c);
```


## Variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| party | [[List]]<[[Character]]> | True |  |
| inv | [[List]]<[[Item]]> | True |  |

## Functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

