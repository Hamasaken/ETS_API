---
title: Status
draft: false
tags:
 - ScriptType
 - ScriptObject
---
# Status : [[EventAware]], [[BaseAsset]]

A Status is a temporary effect on a [[Character]] — a poison, a buff, a shield, and so on. It can last a number of turns (`duration`) and carry a strength (`value`), and it runs script hooks when it is applied, when it is removed, and each turn it ticks. A status can also grant [[Trait]]s to the character while it is active.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| isUnique | [[Bool]] | True | When true, a character can only carry one copy at a time. |
| duration | [[Int]] | False | Turns remaining; counts down each tick, 0 never expires. |
| value | [[Int]] | False | A strength number the status's scripts use. |
| image | [[String]] | False | The status's icon. |
| description | [[String]] | False | The status's description text. |

## Script variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| OnApply | [[Function]] | False | Runs when the status is first applied. |
| OnRemove | [[Function]] | False | Runs when the status is removed. |
| OnTick | [[Function]] | False | Runs each turn while the status is active. |

^9cc4c9



## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Status#^istrait75900597\|IsTrait()]] | [[Bool]] | [[TraitType]] trait | True if the status counts as having a trait (or its group). |
| [[Status#^hastrait-1892446971\|HasTrait()]] | [[Bool]] | [[TraitType]] trait | True if the status has exactly this trait. |
| [[Status#^addtrait-1987476510\|AddTrait()]] | [[Bool]] | [[TraitType]] trait | Gives the status a trait. |
| [[Status#^removetrait-1254612727\|RemoveTrait()]] | [[Bool]] | [[TraitType]] trait | Removes a trait from the status. |

## Script functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |



### IsTrait ([[TraitType]] trait) : [[Bool]]

^istrait75900597

Checks whether the status counts as having a given trait — either exactly that trait, or another one from the same trait group. For an exact match only, use [[Status#^hastrait-1892446971\|HasTrait()]].

> [!Abstract]+ Parameters
> 1. `trait` The trait (or trait group) to check for.

> [!Success]+ Return value
> Returns true if the status has the trait or one from its group.

### HasTrait ([[TraitType]] trait) : [[Bool]]

^hastrait-1892446971

Checks whether the status has exactly the given trait. Unlike [[Status#^istrait75900597\|IsTrait()]], this does not count other traits from the same group.

> [!Abstract]+ Parameters
> 1. `trait` The exact trait to check for.

> [!Success]+ Return value
> Returns true if the status has that exact trait.

### AddTrait ([[TraitType]] trait) : [[Bool]]

^addtrait-1987476510

Gives the status a trait. Nothing happens if it already has that trait.

> [!Abstract]+ Parameters
> 1. `trait` The trait to give the status.

> [!Success]+ Return value
> Returns true if the trait was added, or false if the status already had it.

### RemoveTrait ([[TraitType]] trait) : [[Bool]]

^removetrait-1254612727

Removes a trait from the status.

> [!Abstract]+ Parameters
> 1. `trait` The trait to remove.

> [!Success]+ Return value
> Returns true if the status had that trait and it was removed.

