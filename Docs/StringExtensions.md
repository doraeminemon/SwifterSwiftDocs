# String Extensions


## Table of Contents
| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`base64Decoded`**](#base64decoded) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`base64Encoded`**](#base64encoded) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`camelCased`**](#camelcased) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`containEmoji`**](#containemoji) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`firstCharacter`**](#firstcharacter) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`hasLetters`**](#hasletters) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`hasNumbers`**](#hasnumbers) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`isAlphabetic`**](#isalphabetic) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`isAlphaNumeric`**](#isalphanumeric) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`isEmail`**](#isemail) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`isHttpsUrl`**](#ishttpsurl) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`isHttpUrl`**](#ishttpurl) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`isNumeric`**](#isnumeric) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`lastCharacter`**](#lastcharacter) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`latinized`**](#latinized) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`lines`**](#lines) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`mostCommonCharacter`**](#mostcommoncharacter) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`reversed`**](#reversed) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`bool`**](#bool) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`date`**](#date) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`dateTime`**](#datetime) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`double`**](#double) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`float`**](#float) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`int`**](#int) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`int16`**](#int16) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`int32`**](#int32) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`int64`**](#int64) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`int8`**](#int8) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`url`**](#url) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`trimmed`**](#trimmed) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`unicodeArray`**](#unicodearray) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`urlDecoded`**](#urldecoded) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`urlEncoded`**](#urlencoded) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`withoutSpacesAndNewLines`**](#withoutspacesandnewlines) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`subscript(i: Int)`**]() | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`subscript(range: CountableRange<Int>)`**]() | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`subscript(range: ClosedRange<Int>)`**]() | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`copyToPasteboard()`**]() | Method | 8+ | - | - | 10.10+ |
| [**`camelize()`**]() | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`contain(_ string: String, caseSensitive: Bool)`**]() | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`count(of string: String, caseSensitive: Bool)`**]() | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`end(with suffix: String, caseSensitive: Bool)`**]() | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`firstIndex(of string: String)`**]() | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`latinize()`**]() | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`random(ofLength: Int)`**]() | Static Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`replacing(_ substring: String, with newString: String)`**]() | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`reverse()`**]() | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`slicing(from i: Int, length: Int)`**]() | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`slice(from i: Int, length: Int)`**]() | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`slicing(from start: Int, to end: Int)`**]() | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`slice(from start: Int, to end: Int)`**]() | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`slicing(at i: Int)`**]() | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`slice(at i: Int)`**]() | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`splitted(by separator: Character)`**]() | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`start(with prefix: String, caseSensitive: Bool)`**]() | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`date(withFormat format: String)`**]() | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`trim()`**]() | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`truncate(toLength: Int, trailing: String?)`**]() | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`truncated(toLength: Int, trailing: String?)`**]() | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`urlDecode()`**]() | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`urlEncode()`**]() | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`*`**]() | Infix Operator | 8+ | 9+ | 3+ | 10.10+ |
| [**`init?(base64: String)`**]() | Optional Initializer | 8+ | 9+ | 3+ | 10.10+ |
| [**`bold`**]() | Read-Only Property | 8+ | - | - | 10.10+ |
| [**`underline`**]() | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`strikethrough`**]() | Read-Only Property | 8+ | - | 3+ | 10.10+ |
| [**`italic`**]() | Read-Only Property | 8+ | - | - | - |
| [**`colored(with color: UIColor/NSColor)`**]() | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`nsString`**]() | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`lastPathComponent`**]() | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`pathExtension`**]() | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`deletingLastPathComponent`**]() | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`deletingPathExtension`**]() | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`pathComponents`**]() | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`appendingPathComponent(_ str: String)`**]() | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`appendingPathExtension(_ str: String)`**]() | Method | 8+ | 9+ | 3+ | 10.10+ |

--


## `base64Decoded`
String decoded from base64 (if applicable).

 - **type**: Read-Only Property.
 - **return type**: String?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"SGVsbG8gV29ybGQh".base64Decoded = Optional("Hello World!")
```


--


## `base64Encoded`
String encoded in base64 (if applicable).

 - **type**: Read-Only Property.
 - **return type**: String?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"Hello World!".base64Encoded -> Optional("SGVsbG8gV29ybGQh")
```


--


## `camelCased`
CamelCase of string.

 - **type**: Read-Only Property.
 - **return type**: String
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"sOme vAriable naMe".camelCased -> "someVariableName"
```


--


## `containEmoji`
Check if string contains one or more emojis.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"Hello 😀".containEmoji -> true
```


--


## `firstCharacter`
First character of string (if applicable).

 - **type**: Read-Only Property.
 - **return type**: String?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"Hello".firstCharacter -> Optional("H")
```


--


## `hasLetters`
Check if string contains one or more letters.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"123abc".hasLetters -> true
"abc".hasLetters -> false
```


--


## `hasNumbers`
Check if string contains one or more numbers.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"abcd".hasNumbers -> false
"123abc".hasNumbers -> true
```


--


## `isAlphabetic`
Check if string contains only letters.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"abc".isAlphabetic -> true
"123abc".isAlphabetic -> false
```


--


## `isAlphaNumeric`
Check if string contains at least one letter and one number.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
// useful for passwords
"123abc".isAlphaNumeric -> true
"abc".isAlphaNumeric -> false
```


--


## `isEmail`
Check if string is valid email format.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"john@doe.com".isEmail -> true
```


--


## `isHttpsUrl`
Check if string is https URL.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"https://google.com".isHttpsUrl -> true
```


--


## `isHttpUrl`
Check if string is http URL.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"http://google.com".isHttpUrl -> true
```


--


## `isNumeric`
Check if string contains only numbers.

 - **type**: Read-Only Property.
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"123".isNumeric -> true
"abc".isNumeric -> false
```


--


## `lastCharacter`
Last character of string (if applicable).

 - **type**: Read-Only Property.
 - **return type**: String?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"Hello".lastCharacter -> Optional("o")
```


--


## `latinized`
Latinized string.

 - **type**: Read-Only Property.
 - **return type**: String
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"Hèllö Wórld!".latinized -> "Hello World!"
```


--


## `lines`
Array of strings separated by new lines.

 - **type**: Read-Only Property
 - **return type**: [String]
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"Hello\ntest".lines -> ["Hello", "test"]
```


--


## `mostCommonCharacter`
The most common character in string.

 - **type**: Read-Only Property.
 - **return type**: String
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"This is a test, since e is appearing everywhere e should be the common character".mostCommonCharacter -> "e"
```


--


## `reversed`
Reversed string.

 - **type**: Read-Only Property.
 - **return type**: String
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"Swift".reversed -> "tfiwS"
```


--


## `bool`
Bool value from string (if applicable).

 - **type**: Read-Only Property.
 - **return type**: Bool?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"1".bool -> true
"False".bool -> false
"Hello".bool = nil
```


--


## `date`
Date object from "yyyy-MM-dd" formatted string

 - **type**: Read-Only Property.
 - **return type**: Date?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"2007-06-29".date -> Date?
```


--


## `dateTime`
Date object from "yyyy-MM-dd HH:mm:ss" formatted string.

 - **type**: Read-Only Property.
 - **return type**: Date?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"2007-06-29 14:23:09".dateTime -> Date?
```


--


## `double`
Double value from string (if applicable).

 - **type**: Read-Only Property.
 - **return type**: Double?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"20".double -> 20.0
```


--


## `float`
Float value from string (if applicable).

 - **type**: Read-Only Property.
 - **return type**: Float?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"21".float -> 21.0
```


--


## `float32`
Float32 value from string (if applicable).

 - **type**: Read-Only Property.
 - **return type**: Float32?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"21.86".float32 -> 21.86
```


--


## `float64`
Float64 value from string (if applicable).

 - **type**: Read-Only Property.
 - **return type**: Float64?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"23.45".float64 -> 23.45
```


--


## `int`
Integer value from string (if applicable).

 - **type**: Read-Only Property.
 - **return type**: Int?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"101".int -> 101
```


--


## `int16`
Int16 value from string (if applicable).

 - **type**: Read-Only Property.
 - **return type**: Int16?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"101".int16 -> 101
```


--


## `int32`
Int32 value from string (if applicable).

 - **type**: Read-Only Property.
 - **return type**: Int32?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"101".int32 -> 101
```


--


## `int64`
Int64 value from string (if applicable).

 - **type**: Read-Only Property.
 - **return type**: Int64?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"101".int64 -> 101
```


--


## `int8`
Int8 value from string (if applicable).

 - **type**: Read-Only Property.
 - **return type**: Int8?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"101".int8 -> 101
```


--


## `url`
URL from string (if applicable).

 - **type**: Read-Only Property.
 - **return type**: URL?
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"https://google.com".url -> URL(string: "https://google.com")
"not url".url -> nil
```


--


## `trimmed`
String with no spaces or new lines in beginning and end.

 - **type**: Read-Only Property.
 - **return type**: String
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"   hello  \n".trimmed -> "hello"
```


--


## `unicodeArray`
Array with unicodes for all characters in a string.

 - **type**: Read-Only Property.
 - **return type**: [Int]
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"SwifterSwift".unicodeArray -> [83, 119, 105, 102, 116, 101, 114, 83, 119, 105, 102, 116]
```


--


## `urlDecoded`
Readable string from a URL string.

 - **type**: Read-Only Property.
 - **return type**: String
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"it's%20easy%20to%20encode%20strings".urlDecoded -> "it's easy to encode strings"
```


--


## `urlEncoded`
URL escaped string.

 - **type**: Read-Only Property.
 - **return type**: String
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"it's easy to encode strings".urlEncoded -> "it's%20easy%20to%20encode%20strings"
```


--


## `withoutSpacesAndNewLines`
String without spaces and new lines.

 - **type**: Read-Only Property.
 - **return type**: String
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"   \n Swifter   \n  Swift  ".withoutSpacesAndNewLines -> "SwifterSwift"
```


--


## `subscript(i: Int)`
Safely subscript string with index.

 - **type**: Method.
 - **return type**: String?
 - **parameters**:
   - **i**: index.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"Hello World!"[3] -> "l"
"Hello World!"[20] -> nil
```


--


## `subscript(range: CountableRange<Int>)`
Safely subscript string within a half-open range.

 - **type**: Method.
 - **return type**: String?
 - **parameters**:
  - **range**: Half-open range.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"Hello World!"[6..<11] -> "World"
"Hello World!"[21..<110] -> nil
```


--


## `subscript(range: ClosedRange<Int>)`
Safely subscript string within a closed range.

 - **type**: Method.
 - **return type**: String?
 - **parameters**:
  - **range**: Closed range.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"Hello World!"[6...11] -> "World!"
"Hello World!"[21...110] -> nil
```


--


## `copyToPasteboard()`
Copy string to global pasteboard.

 - **type**: Method.
 - **availability**: `iOS 8+` `macOS 10.10+`.

Example

```swift
"SomeText".copyToPasteboard() // copies "SomeText" to pasteboard
```


--


## `camelize()`
Converts string format to CamelCase.

 - **type**: Mutating Method.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
var str = "sOme vaRiabLe Name"
str.camelize()
print(str) // prints "someVariableName"
```


--


## `contain(_ string: String, caseSensitive: Bool = true)`
Check if string contains one or more instance of substring.

 - **type**: Method.
 - **return type**: Bool
 - **parameters**:
  - **string**: substring to search for.
  - **caseSensitive**: set true for case sensitive search (default is true).
 - **returns**: true if string contains one or more instance of substring. 
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"Hello World!".contain("O") -> false
"Hello World!".contain("o", caseSensitive: false) -> true
```


--


## `count(of string: String, caseSensitive: Bool = true)`
Count of substring in string.

 - **type**: Method.
 - **return type**: Int
 - **parameters**:
  - **string**: substring to search for.
  - **caseSensitive**: set true for case sensitive search (default is true).
 - **returns**: count of appearance of substring in string.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"Hello World!".count(of: "o") -> 2
"Hello World!".count(of: "L", caseSensitive: false) -> 3
```


--


## `end(with suffix: String, caseSensitive: Bool = true)`
Check if string ends with substring.

 - **type**: Method.
 - **return type**: Bool
 - **parameters**:
  - **string**: substring to search if string ends with.
  - **caseSensitive**: set true for case sensitive search (default is true).
 - **returns**: true if string ends with substring.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"Hello World!".end(with: "!") -> true
"Hello World!".end(with: "WoRld!", caseSensitive: false) -> true
```


--


## `firstIndex(of string: String)`
First index of substring in string.

 - **type**: Method.
 - **return type**: Int?
 - **parameters**:
  - **string**: substring to search for.
 - **returns**: first index of substring in string (if applicable).
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"Hello World!".firstIndex(of: "l") -> 2
"Hello World!".firstIndex(of: "s") -> nil
```


--


## `latinize()`
Latinize string.

 - **type**: Mutating Method.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
var str = "Hèllö Wórld!"
str.latinize()
print(str) // prints "Hello World!"
```


--


## `random(ofLength: Int)`
Random string of given length.

 - **type**: Static Method.
 - **return type**: String
 - **parameters**:
  - **ofLength**: number of characters in string.
 - **returns**: random string of given length.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
String.random(ofLength: 18) -> "u7MMZYvGo9obcOcPj8"
```


--


## `replacing(_ substring: String, with newString: String)`
String by replacing part of string with another string.

 - **type**: Method.
 - **return type**: String
 - **parameters**:
  - **substring**: old substring to find and replace.
  - **newString**: new string to insert in old string place.
 - **returns**: string after replacing substring with newString.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
"#number# items".replacing("#number#", with: "10") -> "10 items"
```


--


## `reverse()`
Reverse string.

 - **type**: Mutating Method.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
var str = "Hello World!"
str.reverse()
print(str) // prints "!dlroW olleH"
```


--
