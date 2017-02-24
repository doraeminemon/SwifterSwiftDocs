# Character Extensions


## Table of Contents
| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`isEmoji`**](#isemoji) | Read-Only Property | 8+ | 9+ | 3+ |  10.10+ |
| [**`isNumber`**](#isnumber) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`isUppercased`**](#isuppercased) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`isLowercased`**](#islowercased) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`int`**](#int) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`string`**](#string) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`*`**](#operator-) | Infix Operator | 8+ | 9+ | 3+ | 10.10+ |

--

## `isEmoji`
Check if character is emoji.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`.

Example

```swift
'😀'.isEmoji -> true
```

--

## `isNumber`
Check if character is number.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
'3'.isNumber -> true
```

--

## `isUppercased`
Check if character is uppercased.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
'C'.isUppercased -> true
'c'.isUppercased -> false
```

--

## `isLowercased`
Check if character is lowercased.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
'c'.isLowercased -> true
'C'.isLowercased -> false
```

--

## `int`
Integer from character (if applicable).

 - **type**: Read-Only Property.
 - **return type**: Int?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
'2'.int -> 2
'a'.int -> nil
```

--

## `string`
String from character.

 - **type**: Read-Only Property.
 - **return type**: String
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
'c'.string -> "c"
```

--

## `Operator *`
Repeat character multiple times.

 - **type**: Infix Operator.
 - **return type**: String
 - **returns**: string with character repeated n times.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
'-' * 10 -> "----------"
15 * 'a' -> "aaaaaaaaaaaaaaa"
```
