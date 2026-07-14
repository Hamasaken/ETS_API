---
title: Item
draft: false
tags:
 - ScriptType
 - ScriptObject
---
# Item : [[EventAware]]

An Item is something a [[Character]] can carry, use, consume or equip — a potion, a weapon, a piece of armour. Items carry [[Trait]]s that decide how they can be used, optional [[CombatEffect]]s for what they do in battle, and script hooks (like `OnUse` and `CanEquip`) that run when the player interacts with them.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| image | [[String]] | False | The item's icon or picture. |
| description | [[String]] | False | The item's description text shown to the player. |
| consumeHint | [[String]] | False | Short hint shown for consuming the item. |
| useHint | [[String]] | False | Short hint shown for using the item. |
| equipHint | [[String]] | False | Short hint shown for equipping the item. |

## Script variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| CanConsume | [[Function]] | False | Your check for whether the item can be consumed. |
| CanUse | [[Function]] | False | Your check for whether the item can be used. |
| CanEquip | [[Function]] | False | Your check for whether the item can be equipped. |
| CanUnequip | [[Function]] | False | Your check for whether the item can be unequipped. |
| OnConsume | [[Function]] | False | Runs when the item is consumed. |
| OnUse | [[Function]] | False | Runs when the item is used. |
| OnEquip | [[Function]] | False | Runs when the item is equipped. |
| OnUnequip | [[Function]] | False | Runs when the item is unequipped. |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[Item#^istrait75900597\|IsTrait()]] | [[Bool]] | [[TraitType]] trait | True if the item counts as having a trait (or its group). |
| [[Item#^hastrait-1892446971\|HasTrait()]] | [[Bool]] | [[TraitType]] trait | True if the item has exactly this trait. |
| [[Item#^addtrait-1987476510\|AddTrait()]] | [[Bool]] | [[TraitType]] trait | Gives the item a trait. |
| [[Item#^removetrait-1254612727\|RemoveTrait()]] | [[Bool]] | [[TraitType]] trait | Removes a trait from the item. |
| [[Item#^finish729994674\|Finish()]] | [[Void]] |  | Signals the item has finished its effect. |

## Script functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |



### IsTrait ([[TraitType]] trait) : [[Bool]]

^istrait75900597

Checks whether the item counts as having a given trait — either exactly that trait, or another one from the same trait group. This is how scripts tell what kind of item it is, such as whether it is Consumable or Equipment. For an exact match only, use [[Item#^hastrait-1892446971\|HasTrait()]].

> [!Abstract]+ Parameters
> 1. `trait` The trait (or trait group) to check for.

> [!Success]+ Return value
> Returns true if the item has the trait or one from its group.

### HasTrait ([[TraitType]] trait) : [[Bool]]

^hastrait-1892446971

Checks whether the item has exactly the given trait. Unlike [[Item#^istrait75900597\|IsTrait()]], this does not count other traits from the same group.

> [!Abstract]+ Parameters
> 1. `trait` The exact trait to check for.

> [!Success]+ Return value
> Returns true if the item has that exact trait.

### AddTrait ([[TraitType]] trait) : [[Bool]]

^addtrait-1987476510

Gives the item a trait. Nothing happens if it already has that trait.

> [!Abstract]+ Parameters
> 1. `trait` The trait to give the item.

> [!Success]+ Return value
> Returns true if the trait was added, or false if the item already had it.

### RemoveTrait ([[TraitType]] trait) : [[Bool]]

^removetrait-1254612727

Removes a trait from the item.

> [!Abstract]+ Parameters
> 1. `trait` The trait to remove.

> [!Success]+ Return value
> Returns true if the item had that trait and it was removed.

### Finish () : [[Void]]

^finish729994674

Signals that the item has finished doing its effect, letting whatever triggered it (such as a combat action) carry on. Call this at the end of an item's script once its work is done.

