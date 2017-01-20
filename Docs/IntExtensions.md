# Int Extensions

## Table of Contents
| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`abs`**](#abs) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`asLocaleCurrency`**](#aslocalecurrency) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`degreesToRadians`**](#degreestoradians) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`digits`**](#digits) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`digitsCount`**](#digitscount) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`isEven`**](#iseven) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`isOdd`**](#isodd) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`radiansToDegrees`**](#radianstodegrees) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`romanNumeral`**](#romannumeral) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`timeString`**](#timestring) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`kFormatted`**](#kformatted) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`gcd(of n: Int)`**](#gcdof-n-int) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`lcm(of n: Int)`**](#lcmof-n-int) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`randomBetween(min: Int, max: Int)`**](#randombetweenmin-int-max-int) | Static Method | 8+ | 9+ | 3+ | 10.10+ |
| [**` ** `**](#infix-operator-) | Infix Operator | 8+ | 9+ | 3+ | 10.10+ |
| [**`√`**](#prefix-operator-) | Prefix Operator | 8+ | 9+ | 3+ | 10.10+ |
| [**`±`**](#infix-operator--1) | Infix Operator | 8+ | 9+ | 3+ | 10.10+ |
| [**`±`**](#prefix-operator--1) | Prefix Operator | 8+ | 9+ | 3+ | 10.10+ |


--


## `abs`
Absolute value of integer.

 - **type**: Read-Only Property.
 - **return type**: Int
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
1.abs -> 1
(-1).abs -> 1
```


--


## `asLocaleCurrency`
String with number and current locale currency.

 - **type**: Read-Only Property.
 - **return type**: String
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
1.asLocaleCurrency -> "$1.00"
```


--


## `degreesToRadians`
Radian value of degree input.

 - **type**: Read-Only Property.
 - **return type**: Double
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
180.degreesToRadians -> 3.141592653589793

```


--


## `digits`
Array of digits of integer value.

 - **type**: Read-Only Property.
 - **return type**: [Int]
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
123.digits -> [1, 2, 3]
```


--


## `digitsCount`
Number of digits of integer value.

 - **type**: Read-Only Property.
 - **return type**: Int
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
123.digitsCount = 3
```


--


## `isEven`
Check if integer is even.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
2.isEven -> true
1.isEven -> false
```


--


## `isOdd`
Check if integer is odd.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
1.isOdd -> true
2.isOdd -> false
```


--


## `radiansToDegrees`
Degree value of radian input

 - **type**: Read-Only Property.
 - **return type**: Double
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
1.radiansToDegrees -> 57.29577951308232
```


--


## `romanNumeral`
Roman numeral string from integer (if applicable).

 - **type**: Read-Only Property.
 - **return type**: String?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
13.romanNumeral -> "XIII"
(-6).romanNumeral -> nil
```


--


## `timeString`
String of format (XXh XXm) from seconds Int.

 - **type**: Read-Only Property.
 - **return type**: String
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
13.timeString -> "13 sec"
516.timeString -> "8 min"
4243.timeString -> "1 h 10 m"
```


--


## `kFormatted`
String formatted for values over ±1000 (example: 1k, -2k, 100k, 1kk, -5kk..)

 - **type**: Read-Only Property.
 - **return type**: String
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
13.kFormatted -> "0K"
1209.kFormatted -> "1k"
(-4000).kFormatted -> "-4k"
```


--


## `gcd(of n: Int)`
Greatest common divisor of integer value and n.

 - **type**: Method.
 - **return type**: Int
 - **parameters**:
   - **n**: integer value to find gcd with.
 - **returns**: greatest common divisor of self and n.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
124.gcd(of: 12) -> 4
```


--


## `lcm(of n: Int)`
Least common multiple of integer and n.

 - **type**: Method.
 - **return type**: Int
 - **parameters**:
   - **n**: integer value to find lcm with.
 - **returns**: least common multiple of self and n.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
4.lcm(of: 3) -> 12
```


--


## `randomBetween(min: Int, max: Int)`
Random integer between two integer values.

 - **type**: Static Method.
 - **return type**: type
 - **parameters**:
   - **min**: minimum number to start random from.
   - **max**: maximum number random number end before.
 - **returns**: random integer between two integer values.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
Int.randomBetween(min: 5, max: 25) -> 20
```


--


## `Infix Operator **`
Value of exponentiation.

 - **type**: Infix Operator.
 - **return type**: Double
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
2 ** 3 -> 8
5 ** 2 -> 25
```


--


## `Prefix Operator √`
Square root of integer.

 - **type**: Prefix Operator.
 - **return type**: Double
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
√ 25 -> 5.0
```


--


## `Infix Operator ±`
Tuple of plus-minus operation.

 - **type**: Infix Operator.
 - **return type**: Double
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
2 ± 2 -> (0, 4)
```


--


## `Prefix Operator ±`
Tuple of plus-minus operation.

 - **type**: Infix Operator.
 - **return type**: Double
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
± 2 -> (-2, 2)
```
