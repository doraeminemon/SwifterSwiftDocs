# Array Extensions


## Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`average`**](#average) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`randomItem`**](#randomitem) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`shuffled`**](#shuffled) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`sum`**](#sum) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`withoutDuplicates`**](#withoutduplicates) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`contains(_ elements: [Element])`**](#contains_-elements-element) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`firstIndex <Item: Equatable> (of item: Item)`**](#firstindex-item-equatable-of-item-item) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`indexes(of item: Element)`**](#indexesof-item-element) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`item(at index: Int)`**](#itemat-index-int) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`lastIndex <Item: Equatable> (of item: Item)`**](#lastindex-item-equatable-of-item-item) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`pop()`**](#pop) | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`prepend(_ newElement: Element)`**](#prepend_-newelement-element) | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`push(_ newElement: Element)`**](#push_-newelement-element) | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`safeSwap(from index: Int, to otherIndex: Int)`**](#safeswapfrom-index-int-to-otherIndex-int) | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`swap(from index: Int, to otherIndex: Int)`**](#swapfrom-index-int-to-otherIndex-int) | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`firstIndex(where condition: (Element) -> Bool) -> Int?`**](#firstindexwhere-condition-element---bool---int) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`lastIndex(where condition: (Element) -> Bool) -> Int?`**](#lastindexwhere-condition-element---bool---int) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`indices(where condition: (Element) -> Bool) -> [Int]?`**](#indiceswhere-condition-element---bool---int) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`all(matching condition: (Element) -> Bool) -> Bool?`**](#allmatching-condition-element---bool---bool) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`none(matching condition: (Element) -> Bool) -> Bool?`**](#nonematching-condition-element---bool---bool) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`last(where condition: (Element) -> Bool) -> Element?`**](#lastwhere-condition-element---bool---element) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`reject(where condition: (Element) -> Bool) -> [Element]`**](#rejectwhere-condition-element---bool---element) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`count(where condition: (Element) -> Bool) -> Int`**](#countwhere-condition-element---bool---int) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`forEachReversed(_ body: (Element) -> Void)`**](#foreachreversed_-body-element---void) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`forEach(where condition: (Element) -> Bool, body: (Element) -> Void)`**](#foreachwhere-condition-element---bool-body-element---void) | Method | 8+ | 9+ | 3+ | 10.10+ |  
| [**`removeAll(_ items: [Element])`**](#removeall_-items-element) | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`removeAll(_ item: Element)`**](#removeall_-item-element) | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`removeDuplicates()`**](#removeduplicates) | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`shuffle()`**](#shuffle) | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |


---


## `average`
Average of all elements in array.

 - **type**: Read-Only Property.
 - **return type**: Double
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[1, 2, 3, 4, 5].average = 3.0
[1.2, 2.3, 4.5, 3.4, 4.5].average = 3.18
```


---


## `randomItem`
Random item from array.

 - **type**: Read-Only Property.
 - **return type**: Element
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[1, 2, 3, 4, 5].randomItem // return a random integer from given array.
[1.2, 2.3, 4.5, 3.4, 4.5].randomItem // returns a random double from given array.
["h", "e", "l", "l", "o"].randomItem // returns a random character from given array.
// It also works for all other types!
```


---


## `shuffled`
Shuffled version of array.

 - **type**: Read-Only Property.
 - **return type**: Element
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[1, 2, 3, 4, 5].shuffled // return a shuffled version from given array e.g. [2, 4, 1, 3, 5].
// It also works for all other types!
```


---


## `sum`
Sum of all elements in array.

 - **type**: Read-Only Property.
 - **return type**: Int for int arrays and floating number for floating number arrays.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[1, 2, 3, 4, 5].sum -> 15
[1.2, 2.3, 4.5, 3.4, 4.5].sum -> 15.9
```


---


## `withoutDuplicates`
Array with all duplicates removed from it.

 - **type**: Read-Only Property.
 - **return type**: [Element]
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[1, 2, 2, 3, 4, 5].withoutDuplicates -> [1, 2, 3, 4, 5]
["h", "e", "l", "l", "o"].withoutDuplicates -> ["h", "e", "l", "o"]
// It also works for all other types!
```


---


## `contains(_ elements: [Element])`
Check if array contains an array of elements.

 - **type**: Method.
 - **return type**: Bool
 - **parameters**:
  - **elements**: array of elements to check.
 - **returns**: true if array contains all given items.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[1, 2, 3, 4, 5].contains([1, 2]) -> true
[1.2, 2.3, 4.5, 3.4, 4.5].contains([2, 6]) -> false
["h", "e", "l", "l", "o"].contains(["l", "o"]) -> true
// It also works for all other types!
```


---


## `firstIndex <Item: Equatable> (of item: Item)`
First index of a given item in an array.

 - **type**: Method.
 - **return type**: Int?
 - **parameters**:
  - **item**: item to check.
 - **returns**: first index of item in array (if exists).
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[1, 2, 2, 3, 4, 2, 5].firstIndex(of 2) -> 1
[1.2, 2.3, 4.5, 3.4, 4.5].firstIndex(of 6.5) -> nil
["h", "e", "l", "l", "o"].firstIndex(of "l") -> 2
// It also works for all other types!
```


---


## `indexes(of item: Element)`
All indexes of specified item.

 - **type**: Method.
 - **return type**: [Int]
 - **parameters**:
  - **item**: item to check.
 - **returns**: an array with all indexes of the given item.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[1, 2, 2, 3, 4, 2, 5].indexes(of 2) -> [1, 2, 5]
[1.2, 2.3, 4.5, 3.4, 4.5].indexes(of 2.3) -> [1]
["h", "e", "l", "l", "o"].indexes(of "l") -> [2, 3]
// It also works for all other types!
```


---


## `item(at index: Int)`
Element at the given index if it exists.

 - **type**: Method.
 - **return type**: Element?
 - **parameters**:
  - **index**: index of element.
 - **returns**: optional element (if exists).
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[1, 2, 3, 4, 5].item(at: 2) -> 3
[1.2, 2.3, 4.5, 3.4, 4.5].item(at: 3) -> 3.4
["h", "e", "l", "l", "o"].item(at: 10) -> nil
// It also works for all other types!
```


---


## `lastIndex <Item: Equatable> (of item: Item)`
Last index of a given item in an array.

 - **type**: Method.
 - **return type**: Int?
 - **parameters**:
  - **item**: item to check.
 - **returns**: last index of item in array (if exists).
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[1, 2, 2, 3, 4, 2, 5].lastIndex(of 2) -> 5
[1.2, 2.3, 4.5, 3.4, 4.5].lastIndex(of 6.5) -> nil
["h", "e", "l", "l", "o"].lastIndex(of "l") -> 3
// It also works for all other types!
```


---


## `pop()`
Remove last element from array and return it.

 - **type**: Mutating Method.
 - **return type**: Element?
 - **returns**: last element in array (if applicable).
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[1, 2, 3, 4, 5].pop() // returns 5 and remove it from the array.
[].pop() // returns nil since the array is empty.
// It also works for all other types!
```


---


## `prepend(_ newElement: Element)`
Insert an element at the beginning of array.

 - **type**: Method.
 - **parameters**:
  - **newElement**: element to insert.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[2, 3, 4, 5].prepend(1) -> [1, 2, 3, 4, 5]
["e", "l", "l", "o"].prepend("h") -> ["h", "e", "l", "l", "o"]
// It also works for all other types!
```


---


## `push(_ newElement: Element)`
Insert an element to the end of array.

 - **type**: Method.
 - **parameters**:
  - **newElement**: element to insert.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[1, 2, 3, 4].push(5) -> [1, 2, 3, 4, 5]
["h", "e", "l", "l"].push("o") -> ["h", "e", "l", "l", "o"]
// It also works for all other types!
```


---


## `safeSwap(from index: Int, to otherIndex: Int)`
Safely Swap values at index positions.

 - **type**: Method.
 - **parameters**:
  - **index**: index of first element.
  - **otherIndex**: index of other element.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.
 
Example

```swift
[1, 2, 3, 4, 5].safeSwap(from: 3, to: 0) -> [4, 2, 3, 1, 5]
["h", "e", "l", "l", "o"].safeSwap(from: 1, to: 0) -> ["e", "h", "l", "l", "o"]
// It also works for all other types!
```


---


## `swap(from index: Int, to otherIndex: Int)`
Swap values at index positions. Doesn't check index range.

 - **type**: Method.
 - **parameters**:
  - **index**: index of first element.
  - **otherIndex**: index of other element.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.
 
Example

```swift
[1, 2, 3, 4, 5].swap(from: 3, to: 0) -> [4, 2, 3, 1, 5]
["h", "e", "l", "l", "o"].swap(from: 1, to: 0) -> ["e", "h", "l", "l", "o"]
// It also works for all other types!
```


---


## `firstIndex(where condition: (Element) -> Bool) -> Int?`
Get first index where condition is met.

 - **type**: Method.
 - **parameters**:
  - **condition**: condition to evaluate each element against.
 - **returns**: first index where the specified condition evaluates to true. (optional)
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[1, 7, 1, 2, 4, 1, 6].firstIndex { $0 % 2 == 0 } -> 3
// It also works for all other types!
```


---


## `lastIndex(where condition: (Element) -> Bool) -> Int?`
Get last index where condition is met.

 - **type**: Method.
 - **parameters**:
  - **condition**: condition to evaluate each element against.
 - **returns**: last index where the specified condition evaluates to true. (optional)
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[1, 7, 1, 2, 4, 1, 8].lastIndex { $0 % 2 == 0 } -> 6
// It also works for all other types!
```


---


## `indices(where condition: (Element) -> Bool) -> [Int]?`
Get all indices where condition is met.

 - **type**: Method.
 - **parameters**:
  - **condition**: condition to evaluate each element against.
 - **returns**: all indices where the specified condition evaluates to true. (optional)
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[1, 7, 1, 2, 4, 1, 8].indices(where: { $0 == 1 }) -> [0, 2, 5]
// It also works for all other types!
```


---


## `all(matching condition: (Element) -> Bool) -> Bool?`
Check if all elements in array match a conditon.

 - **type**: Method.
 - **parameters**:
  - **condition**: condition to evaluate each element against.
 - **returns**: true when all elements in the array match the specified condition.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[2, 2, 4].all(matching: {$0 % 2 == 0}) -> true
[1,2, 2, 4].all(matching: {$0 % 2 == 0}) -> false
// It also works for all other types!
```

---



## `none(matching condition: (Element) -> Bool) -> Bool?`
Check if no elements in array match a conditon.

 - **type**: Method.
 - **parameters**:
  - **condition**: condition to evaluate each element against.
 - **returns**: true when no elements in the array match the specified condition.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[2, 2, 4].none(matching: {$0 % 2 == 0}) -> false
[1, 3, 5, 7].none(matching: {$0 % 2 == 0}) -> true
// It also works for all other types!
```

---


## `last(where condition: (Element) -> Bool) -> Element?`
Get last element that satisfies a conditon.

 - **type**: Method.
 - **parameters**:
  - **condition**: condition to evaluate each element against.
 - **returns**: the last element in the array matching the specified condition. (optional)
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[2, 2, 4, 7].last(where: {$0 % 2 == 0}) -> 4
// It also works for all other types!
```

---


## `reject(where condition: (Element) -> Bool) -> [Element]`
Filter elements based on a rejection condition.

 - **type**: Method.
 - **parameters**:
  - **condition**: to evaluate the exclusion of an element from the array.
 - **returns**: the array with rejected values filtered from it.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[2, 2, 4, 7].reject(where: {$0 % 2 == 0}) -> [7]
// It also works for all other types!
```

---


## `count(where condition: (Element) -> Bool) -> Int`
Get element count based on condition.

 - **type**: Method.
 - **parameters**:
  - **condition**: condition to evaluate each element against.
 - **returns**: number of times the condition evaluated to true.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[2, 2, 4, 7].count(where: {$0 % 2 == 0}) -> 3
// It also works for all other types!
```

---


## `forEachReversed(_ body: (Element) -> Void)` 
Iterate over a collection in reverse order. (right to left)

 - **type**: Method.
 - **parameters**:
  - **body**: a closure that takes an element of the array as a parameter.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[0, 2, 4, 7].forEachReversed({ print($0)}) -> //Order of print: 7,4,2,0
// It also works for all other types!
```

---


## `forEach(where condition: (Element) -> Bool, body: (Element) -> Void)`
Calls given closure with each element where condition is true.

 - **type**: Method.
 - **parameters**:
  - **condition**: condition to evaluate each element against.
  - **body**: a closure that takes an element of the array as a parameter.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[0, 2, 4, 7].forEach( where: {$0 % 2 == 0}, body: { print($0)}) -> //print: 0, 2, 4
// It also works for all other types!
```

---


## `removeAll(_ item: Element)`
Remove all instances of an item from array.

 - **type**: Mutating Method.
 - **parameters**:
  - **item**: item to remove.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[1, 2, 2, 3, 4, 5].removeAll(2) -> [1, 3, 4, 5]
["h", "e", "l", "l", "o"].removeAll("l") -> ["h", "e", "o"]
// It also works for all other types!
```


---


## `removeAll(_ items: [Element])`
Remove all instances contained in items parameter from array.

 - **type**: Mutating Method.
 - **parameters**:
  - **items**: iitems to remove.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[1, 2, 2, 3, 4, 5].removeAll([2,5]) -> [1, 3, 4]
["h", "e", "l", "l", "o"].removeAll(["l", "h"]) -> ["e", "o"]
// It also works for all other types!
```


---


## `removeDuplicates()`
Remove all duplicates from array.

 - **type**: Mutating Method.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[1, 2, 2, 3, 4, 5].removeDuplicates() -> [1, 2, 3, 4, 5]
["h", "e", "l", "l", "o"]. removeDuplicates() -> ["h", "e", "l", "o"]
// It also works for all other types!
```


---


## `shuffle()`
Shuffle array.

 - **type**: Mutating Method.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
[1, 2, 3, 4, 5].shuffle() // shuffles array
// It also works for all other types!
```


---
