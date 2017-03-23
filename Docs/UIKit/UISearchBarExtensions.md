# UISearchBar Extensions

## Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`textField`**](#textfield) | Read-Only Property | 8+ | 9+ | - | - |
| [**`trimmedText`**](#trimmedtext) | Read-Only Property | 8+ | 9+ | - | - |
| [**`clear()`**](#clear) | Method | 8+ | 9+ | - | - |


---


## `textField`
Text field inside search bar (if applicable).

- **type**: Read-Only Property.
- **return type**: UITextField?
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let searchBar = UISearchBar()
let textField = searchBar.textField
```

---

## `trimmedText`
Text with no spaces or new lines in beginning and end (if applicable).

- **type**: Read-Only Property.
- **return type**: String?
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let searchBar = UISearchBar()
let trimmedText = searchBar.trimmedText
```

---

## `clear()`
Clear text.

- **type**: Method.
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let searchBar = UISearchBar()
searchBar.clear()
```


---
