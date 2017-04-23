# Locale Extensions


## Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`posix`**](#int) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |


---


## `posix`
UNIX representation of locale usually used for normalizing.

 - **type**: Read-Only Property.
 - **return type**: Locale
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
let dateFormatter = DateFormatter()
dateFormatter.locale = .posix
```


---
