# Double Extensions


## Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`abs`**](#abs) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`asLocaleCurrency`**](#aslocalecurrency) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`ceil`**](#ceil) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`degreesToRadians`**](#degreestoradians) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`floor`**](#floor) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`radiansToDegrees`**](#radianstodegrees) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`randomBetween(min: Double, max: Double)`**](#) | Static Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`randomBetween(min: Double, max: Double)`**](#randombetweenmin-double-max-double) | Static Method | 8+ | 9+ | 3+ | 10.10+ |
| [**` ** `**](#operator-) | Infix Operator | 8+ | 9+ | 3+ | 10.10+ |
| [**`√`**](#operator--1) | Prefix Operator | 8+ | 9+ | 3+ | 10.10+ |
| [**`±`**](#operator--2) | Prefix/Infix Operator | 8+ | 9+ | 3+ | 10.10+ |


--


## `abs`
Absolute of double value.

 - **type**: Read-Only Property.
 - **return type**: Double
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
Double(12.12) -> 12.12
Double(-12.12) -> 12.12
```


--


## `asLocaleCurrency`
String with number and current locale currency.

 - **type**: Read-Only Property.
 - **return type**: String
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
Double(12.12).asLocaleCurrency -> "$12.12"
Double(10).asLocaleCurrency ->"$10.00"
```


--


## `ceil`
Ceil of double value.

 - **type**: Read-Only Property.
 - **return type**: Double
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
Double(12.12).ceil -> 13
Double(-12.12).ceil -> -12
Double(10).ceil -> 10
```


--



## `degreesToRadians`
Radian value of degree input.

 - **type**: Read-Only Property.
 - **return type**: Double
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
Double(180).degreesToRadians -> M_PI
```


--


## `floor`
Floor of double value.

 - **type**: Read-Only Property.
 - **return type**: Double
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
Double(12.12).floor -> 12
Double(-12.12).floor -> -13
Double(10).floor -> 10
```


--


## `radiansToDegrees`
Degree value of radian input.

 - **type**: Read-Only Property.
 - **return type**: Double
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
M_PI.radiansToDegrees -> 180.0
```


--


## `randomBetween(min: Double, max: Double)`
Converts string format to CamelCase.

 - **type**: Static Method.
 - **return type**: Double
 - **parameters**:
 	- **min**: minimum number to start random from.
 	- **max**: maximum number random number end before.
 - **returns**: random double between two double values.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
Double.randomBetween(min: 1, max: 10) -> random double number between 1 and 10
```


--


## `Operator **`
Value of exponentiation.

 - **type**: Infix Operator.
 - **return type**: Double
 - **parameters**:
 	- **lhs**: base double.
 	- **rhs**: exponent double.
 - **returns**: exponentiation result.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
2.0 ** 2.0 -> 4.0
4.4 ** 0.5 -> 2.0976176963
```


--


## `Operator √`
Square root of double.

 - **type**: Prefix Operator.
 - **return type**: Double
 - **parameters**:
 	- **double**: double value to find square root for.
 - **returns**: square root of given double.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
√ 4.0 -> 2.0
```


--


## `Operator ±`
Tuple of plus-minus operation.

 - **type**: Prefix/Infix Operator.
 - **return type**: Double
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
5.0 ± 2.0 -> (3.0, 7.0)
± 2.0 -> (2.0, -2.0)
```
