# Character Extensions


## Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`isEmoji`**](#isemoji) | Read-Only Property | 8+ | 9+ | 3+ |  10.10+ |
| [**`isNumber`**](#isnumber) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`isLetter`**](#isletter) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`isUppercased`**](#isuppercased) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`isLowercased`**](#islowercased) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`isWhiteSpace`**](#iswhitespace) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`int`**](#int) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`string`**](#string) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`lowercased`**](#lowercased) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`uppercased`**](#uppercased) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`*`**](#operator-) | Infix Operator | 8+ | 9+ | 3+ | 10.10+ |


---


## `isEmoji`
Check if character is emoji.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`.

Example

```swift
'😀'.isEmoji -> true
```


---


## `isNumber`
Check if character is number.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
'3'.isNumber -> true
```


---



## `isLetter`
Check if character is a letter.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
'3'.isLetter -> false
'a'.isLetter -> true
```


---
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


---


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


---


## `isWhiteSpace`
Check if character is white space.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
' '.isWhiteSpace -> true
'C'.isWhiteSpace -> false
```


---


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


---


## `string`
String from character.

 - **type**: Read-Only Property.
 - **return type**: String
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
'c'.string -> "c"
```


---


## `lowercased`
Return the character lowercased.

 - **type**: Read-Only Property.
 - **return type**: Character
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
'A'.lowercased -> "a"
```


---


## `uppercased`
Return the character uppercased.

 - **type**: Read-Only Property.
 - **return type**: Character
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
'b'.uppercased -> "B"
```


---
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

---
