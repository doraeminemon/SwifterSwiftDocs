# Collection Extensions


## Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`forEachInParallel(_ each: (Self.Iterator.Element) -> ())`**](#foreachinparallel_-each-selfiteratorelement---) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`subscript (safe index: Index)`**](#subscript-safe-index-index) | Method | 8+ | 9+ | 3+ | 10.10+ |


---


## `forEachInParallel(_ each: (Self.Iterator.Element) -> ())`
Performs `each` closure for each element of collection in parallel.

 - **type**: Method.
 - **parameters**:
  - **each**: closure to run for each element.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
array.forEachInParallel { item in
	print(item)
}
```


---


## `subscript (safe index: Index)`
Safe protects the array from out of bounds by use of optional.

 - **type**: Method.
 - **return type**: Generator.Element?
 - **parameters**:
  - **index**: Index of element to access element.
 - **returns**: Optional element at index (if applicable).
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
let arr = [1, 2, 3, 4, 5]
arr[safe: 1] -> 2
arr[safe: 10] -> nil
```


---
