# String Extensions


## Table of Contents
| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`base64Decoded`**](#base64decoded) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`base64Encoded`**](#base64encoded) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`camelCased`**](#camelcased) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`containEmoji`**](#containemoji) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`firstCharacter`**](#firstcharacter) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`hasLetters`**](#hasletters) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`hasNumbers`**](#hasnumbers) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`isAlphabetic`**](#isalphabetic) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`isAlphaNumeric`**](#isalphanumeric) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`isEmail`**](#isemail) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`isHttpsUrl`**](#ishttpsurl) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`isHttpUrl`**](#ishttpurl) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`isNumeric`**](#isnumeric) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`lastCharacter`**](#lastcharacter) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`latinized`**](#latinized) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`lines`**](#lines) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`mostCommonCharacter`**](#mostcommoncharacter) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`reversed`**](#reversed) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`bool`**](#bool) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`date`**](#date) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`dateTime`**](#datetime) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`double`**](#double) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`float`**](#float) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`float32`**](#float32) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`float64`**](#float64) | Read-Only Property | 8+ | 9+ | 3+ | NA|
| [**`replacing(substring, with: newString)`**](#replacing_-substring-string-with-newstring-string) | Method | 8+ | 9+ | 3+ | NA|

--

## `base64Decoded`
String decoded from base64  (if applicable).

 - **type**: Read-Only Property.
 - **return type**: String?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"SGVsbG8gV29ybGQh".base64Decoded = Optional("Hello World!")
```

--

## `base64Encoded`
String encoded in base64 (if applicable).

 - **type**: Read-Only Property.
 - **return type**: String?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"Hello World!".base64Encoded -> Optional("SGVsbG8gV29ybGQh")
```

--

## `camelCased`
CamelCase of string.

 - **type**: Read-Only Property.
 - **return type**: String
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"sOme vAriable naMe".camelCased -> "someVariableName"
```

--

## `containEmoji`
Check if string contains one or more emojis.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"Hello 😀".containEmoji -> true
```

--

## `firstCharacter`
First character of string (if applicable).

 - **type**: Read-Only Property.
 - **return type**: String?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"Hello".firstCharacter -> Optional("H")
```

--

## `hasLetters`
Check if string contains one or more letters.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"123abc".hasLetters -> true
```

--

## `hasNumbers`
Check if string contains one or more numbers.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+`
 - **unit tests**: `iOS`

Example

```swift
"abcd".hasNumbers -> false
```

--

## `isAlphabetic`
Check if string contains only letters.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"abc".isAlphabetic -> true
```

--

## `isAlphaNumeric`
Check if string contains at least one letter and one number.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"123abc".isAlphaNumeric -> true
```

--

## `isEmail`
Check if string is valid email format.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"john@doe.com".isEmail -> true
```

--

## `isHttpsUrl`
Check if string is https URL.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"https://google.com".isHttpsUrl -> true
```

--

## `isHttpUrl`
Check if string is http URL.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"http://google.com".isHttpUrl -> true
```

--

## `isNumeric`
Check if string contains only numbers.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"123".isNumeric -> true
```

--

## `lastCharacter`
Last character of string (if applicable).

 - **type**: Read-Only Property.
 - **return type**: String?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"Hello".lastCharacter -> Optional("o")
```

--

## `latinized`
Latinized string.

 - **type**: Read-Only Property.
 - **return type**: String
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"Hèllö Wórld!".latinized -> "Hello World!"
```

--

## `lines`
Array of strings separated by new lines.

 - **type**: Read-Only Property
 - **return type**: [String]
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"Hello\ntest".lines -> ["Hello", "test"]
```

--

## `mostCommonCharacter`
The most common character in string.

 - **type**: Read-Only Property.
 - **return type**: String
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"This is a test, since e is appearing everywhere e should be the common character".mostCommonCharacter -> "e"
```

--

## `reversed`
Reversed string.

 - **type**: Read-Only Property.
 - **return type**: String
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"Swift".reversed -> "tfiwS"
```

--

## `bool`
Bool value from string (if applicable).

 - **type**: Read-Only Property.
 - **return type**: Bool?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"1".bool -> true
```

--

## `date`
Date object from "yyyy-MM-dd" formatted string

 - **type**: Read-Only Property.
 - **return type**: Date?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"2007-06-29".date -> Date?
```

--

## `dateTime`
Date object from "yyyy-MM-dd HH:mm:ss" formatted string.

 - **type**: Read-Only Property.
 - **return type**: Date?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"2007-06-29 14:23:09".dateTime -> Date?
```

--

## `double`
Double value from string (if applicable).

 - **type**: Read-Only Property.
 - **return type**: Double?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"20".double -> 20.0
```

--

## `float`
Float value from string (if applicable).

 - **type**: Read-Only Property.
 - **return type**: Float?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"21".float -> 21.0
```

--

## `float32`
Float32 value from string (if applicable).

 - **type**: Read-Only Property.
 - **return type**: Float32?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"21.86".float32 -> 21.86
```

--

## `float64`
Float64 value from string (if applicable).

 - **type**: Read-Only Property.
 - **return type**: Float64?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"23.45".float64 -> 23.45
```

--

## `replacing(_ substring: String, with newString: String)`
String by replacing part of string with another string.

 - **type**: Method.
 - **return type**: String
 - **parameters**:
   - `substring`: old substring to find and replace
   - `newString`: new string to insert in old string place
 - **returns**: string after replacing substring with newString
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+`
 - **unit tests**: `iOS`

Example

```swift
"%number% items".replacing("%number%", with: "10") -> "10 items"
```
