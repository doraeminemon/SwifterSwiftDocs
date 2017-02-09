# Float Extensions


## Table of Contents
| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`abs`**](#abs) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`asLocaleCurrency`**](#aslocalecurrency) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`ceil`**](#ceil) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`degreesToRadians`**](#degreestoradians) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`floor`**](#floor) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`radiansToDegrees`**](#radianstodegrees) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`randomBetween(min: Float, max: Float)`**](#) | Static Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`√`**](#) | Prefix Operator | 8+ | 9+ | 3+ | 10.10+ |
| [**`**`**](#) | Infix Operator | 8+ | 9+ | 3+ | 10.10+ |
| [**`±`**](#) | Prefix/Infix Operator | 8+ | 9+ | 3+ | 10.10+ |


--


## `abs`
Absolute of Float value.

 - **type**: Read-Only Property.
 - **return type**: Float
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
Float(12.12) -> 12.12
Float(-12.12) -> 12.12
```


--


## `asLocaleCurrency`
String with number and current locale currency.

 - **type**: Read-Only Property.
 - **return type**: String
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
Float(12.12).asLocaleCurrency -> "$12.12"
Float(10).asLocaleCurrency ->"$10.00"
```


--


## `ceil`
Ceil of Float value.

 - **type**: Read-Only Property.
 - **return type**: Float
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
Float(12.12).ceil -> 13
Float(-12.12).ceil -> -12
Float(10).ceil -> 10
```


--



## `degreesToRadians`
Radian value of degree input.

 - **type**: Read-Only Property.
 - **return type**: Float
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
Float(180).degreesToRadians -> M_PI
```


--


## `floor`
Floor of Float value.

 - **type**: Read-Only Property.
 - **return type**: Float
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
Float(12.12).floor -> 12
Float(-12.12).floor -> -13
Float(10).floor -> 10
```


--


## `radiansToDegrees`
Degree value of radian input.

 - **type**: Read-Only Property.
 - **return type**: Float
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
M_PI.radiansToDegrees -> 180.0
```


--


## `randomBetween(min: Float, max: Float)`
Converts string format to CamelCase.

 - **type**: Static Method.
 - **return type**: Float
 - **parameters**:
 	- **min**: minimum number to start random from.
 	- **max**: maximum number random number end before.
 - **returns**: random Float between two Float values. 
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
Float.randomBetween(min: 1, max: 10) -> random float number between 1 and 10

```


--


## `Operator **`
Value of exponentiation.

 - **type**: Infix Operator.
 - **return type**: Float
 - **parameters**:
 	- **lhs**: base Float.
 	- **rhs**: exponent Float.
 - **returns**: exponentiation result.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
2.0 ** 2.0 -> 4.0
4.4 ** 0.5 -> 2.0976176963
```


--


## `Operator √`
Square root of Float.

 - **type**: Prefix Operator.
 - **return type**: Float
 - **parameters**:
 	- **Float**: Float value to find square root for.
 - **returns**: square root of given Float.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
√ 4.0 -> 2.0
```


--


## `Operator ±`
Tuple of plus-minus operation.

 - **type**: Prefix/Infix Operator.
 - **return type**: Float
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
5.0 ± 2.0 -> (3.0, 7.0)
± 2.0 -> (2.0, -2.0)
```

