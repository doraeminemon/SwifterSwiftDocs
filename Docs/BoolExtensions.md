# Bool Extensions


## Table of Contents
| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`int`**](#int) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`string`**](#string) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`toggled`**](#int) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`toggle()`**](#toggle()) | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |

--

## `int`
Return 1 if true, or 0 if false.

 - **type**: Read-Only Property.
 - **return type**: Int
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
true.int -> 1
```

--

## `string`
Return "true" if true, or "false" if false.

 - **type**: Read-Only Property.
 - **return type**: String
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
false.string -> "false"
```

--

## `toggled`
Return inversed value of bool.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
false.toggled -> true
```

--

## `toggle()`
Toggle value for bool.

 - **type**: Mutating Method.
 - **return type**: Bool
 - **returns**: inversed value of bool.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
var x = true
x.toggle()
print(x) -> false
```
