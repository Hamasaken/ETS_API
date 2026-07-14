---
title: List
draft: false
tags:
 - ScriptType
---
# List : [[Any]]

A List is an ordered collection of values kept together in one place — the characters in a party, the tiles within an ability's range, the units an attack will hit. The items stay in the order they were added, and you can add to the list, remove from it, look through it, and produce filtered or sorted copies of it. A list can hold values of any type.

## Static variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |

## Prototype variables
| Name | Type | Readonly | Note |
| ---- | ---- | -------- | ---- |
| Count | [[Int]] | True | How many items are currently in the list. |


## Static functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |

## Prototype functions
| Name | Return type | Parameters | Note |
| ---- | ----------- | ---------- | ---- |
| [[List#^clear1844699128\|Clear()]] | [[Void]] |  | Removes every item from the list. |
| [[List#^insert-1425258897\|Insert()]] | [[Void]] | [[Int]] index, [[Any]] object | Adds an item at a specific position. |
| [[List#^add-2138638556\|Add()]] | [[Int]] | [[Any]] object | Adds an item to the end of the list. |
| [[List#^remove-980189283\|Remove()]] | [[Void]] | [[Any]] object | Takes an item out of the list. |
| [[List#^contains-2139094790\|Contains()]] | [[Bool]] | [[Any]] object | True if the item is in the list. |
| [[List#^indexof1066720058\|IndexOf()]] | [[Int]] | [[Any]] object | Position of an item in the list. |
| [[List#^clone540739042\|Clone()]] | [[List]]<[[Any]]> |  | Makes an independent copy of the list. |
| [[List#^where2061106082\|Where()]] | [[List]] | [[Lambda]] filter | Keeps only the items that pass a test. |
| [[List#^orderby-730234582\|OrderBy()]] | [[List]] | [[Lambda]] sortValue | Sorts the items lowest-first. |
| [[List#^orderbydesc-968153573\|OrderByDesc()]] | [[List]] | [[Lambda]] sortValue | Sorts the items highest-first. |



### Clear () : [[Void]]

^clear1844699128

Empties the list, removing all of its items at once. The list itself remains, but afterwards it contains nothing.

### Insert ([[Int]] index, [[Any]] object) : [[Void]]

^insert-1425258897

Adds an item into the list at a specific position, sliding the items already at or after that position along to make room. Positions are counted from 0, so inserting at 0 puts the item at the very front.

> [!Abstract]+ Parameters
> 1. `index` Where to put the item, counted from 0 (0 is the front of the list).
> 2. `object` The value to add.

### Add ([[Any]] object) : [[Int]]

^add-2138638556

Adds an item onto the end of the list.

> [!Example]+ Example
> Add a summoned character to the player's party:
> ```js
> Adventure.party.Add(c)
> ```

> [!Abstract]+ Parameters
> 1. `object` The value to add to the list.

> [!Success]+ Return value
> Returns the position the new item ended up at.

### Remove ([[Any]] object) : [[Void]]

^remove-980189283

Takes the given item back out of the list. If the same value appears more than once, the first match is removed.

> [!Abstract]+ Parameters
> 1. `object` The value to remove from the list.

### Contains ([[Any]] object) : [[Bool]]

^contains-2139094790

Checks whether the given item is somewhere in the list.

> [!Abstract]+ Parameters
> 1. `object` The value to look for.

> [!Success]+ Return value
> Returns true if the item is in the list.

### IndexOf ([[Any]] object) : [[Int]]

^indexof1066720058

Finds where the given item sits in the list and returns its position, counted from 0. Returns -1 when the item isn't in the list at all.

> [!Abstract]+ Parameters
> 1. `object` The value to find.

> [!Success]+ Return value
> Returns the position of the first match, or -1 if the item is not in the list.

### Clone () : [[List]]<[[Any]]>

^clone540739042

Makes a separate copy of the list containing the same items. Because it is independent, adding to or removing from the copy does not change the original (and vice-versa).

> [!Success]+ Return value
> Returns a new list with the same items as this one.

### Where ([[Lambda]] filter) : [[List]]

^where2061106082

Returns a new list containing only the items that pass a test. The test is written as a lambda that receives each item and returns true to keep it or false to drop it. The original list is left unchanged.

> [!Example]+ Example
> Keep only the even numbers in a list:
> ```js
> l3.Where(q => q % 2 == 0)
> ```

> [!Abstract]+ Parameters
> 1. `filter` A test, given each item, that returns true to keep it.

> [!Success]+ Return value
> Returns a new list of just the items that passed the test.

### OrderBy ([[Lambda]] sortValue) : [[List]]

^orderby-730234582

Returns a new list with the same items sorted from lowest to highest. For each item, the given lambda works out the number to sort by. The original list is left unchanged.

> [!Example]+ Example
> Sort a list of numbers from smallest to largest:
> ```js
> l3.OrderBy(q => q)
> ```

> [!Abstract]+ Parameters
> 1. `sortValue` Given each item, works out the number to sort it by.

> [!Success]+ Return value
> Returns a new list sorted lowest-first.

### OrderByDesc ([[Lambda]] sortValue) : [[List]]

^orderbydesc-968153573

Returns a new list with the same items sorted from highest to lowest — the reverse of [[List#^orderby-730234582\|OrderBy()]]. For each item, the given lambda works out the number to sort by. The original list is left unchanged.

> [!Abstract]+ Parameters
> 1. `sortValue` Given each item, works out the number to sort it by.

> [!Success]+ Return value
> Returns a new list sorted highest-first.

