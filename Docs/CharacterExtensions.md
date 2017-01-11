# Character Extensions


## Table of Contents
| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`isEmoji`**](#isemoji) | Read-Only Property | 8+ | 9+ | 3+ | NA |
| [**`isNumber`**](#isnumber) | Read-Only Property | 8+ | 9+ | 3+ | NA |
| [**`int`**](#int) | Read-Only Property | 8+ | 9+ | 3+ | NA |
| [**`string`**](#string) | Read-Only Property | 8+ | 9+ | 3+ | NA |
| [**`*`**](#*) | Infix Operator | 8+ | 9+ | 3+ | NA |

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
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`.

Example

```swift
'3'.isNumber -> true
```

--

## `int`
Integer from character (if applicable).

 - **type**: Read-Only Property.
 - **return type**: Int?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`

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
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`

Example

```swift
'c'.string -> "c"
```

--

## `* Operator`
Repeat character multiple times.

 - **type**: Infix Operator.
 - **return type**: String
 - **returns**: string with character repeated n times.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`

Example

```swift
'-' * 10 -> "----------"
15 * 'a' -> "aaaaaaaaaaaaaaa"
```
