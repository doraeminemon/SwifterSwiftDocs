## String Extensions

### Table of Contents
| Name | Type |
|:--- | :--- |
| [**`base64Decoded`**](#base64decoded) | Read-Only Property |
| [**`base64Encoded`**](#base64encoded) | Read-Only Property |
| [**`camelCased`**](#camelcased) | Read-Only Property |
| [**`containEmoji`**](#containemoji) | Read-Only Property |
| [**`contain(string, caseSensitive)`**](#contain_-string-string-casesensitive-bool--true) | Method | 8+ | 9+ | NA | NA|
| [**`replacing(substring, with newString)`**](#replacing_-substring-string-with-newstring-string) | Method | 8+ | 9+ | NA | NA|

--

### `base64Decoded`
String decoded from base64 (read-Only, if applicable).
 - **type**: Read-Only Property
 - **return type**: String?
 - **availability**: `iOS 8+` `tvOS 9+`
 - **unit tests**: `iOS`

Example
```swift
"SGVsbG8gV29ybGQh".base64Decoded = Optional("Hello World!")
```

--

### `base64Encoded`
String encoded in base64 (read-Only, if applicable).
 - **type**: Read-Only Property
 - **return type**: String?
 - **availability**: `iOS 8+` `tvOS 9+`
 - **unit tests**: `iOS`

Example
```swift
"Hello World!".base64Encoded -> Optional("SGVsbG8gV29ybGQh")
```

--

### `camelCased`
CamelCase of string.
 - **type**: Read-Only Property
 - **return type**: String
 - **availability**: `iOS 8+` `tvOS 9+`
 - **unit tests**: `iOS`

Example
```swift
"Some variable nAme".camelCased -> "someVariableName"
```

--

### `containEmoji`
Check if string contains one or more emojis.
 - **type**: Read-Only Property
 - **return type**: Bool
 - **availability**: `iOS 8+` `tvOS 9+`
 - **unit tests**: `iOS`

Example
```swift
"string👨‍with😍emojis✊🏿".containEmoji -> true
```

--

### `contain(_ string: String, caseSensitive: Bool = true)`
Check if string contains one or more instance of substring.

 - **type**: Method
 - **return type**: Bool
 - **parameters**:
   - **string**: substring to search for.
   - **caseSensitive**: set true for case sensitive search (default is true).
 - **returns**: true if string contains one or more instance of substring.
 - **availability**: `iOS 8+` `tvOS 9+`
 - **unit tests**: `iOS`

Example
```swift
"Hello World!".contain("o", caseSensitive: false) -> true
```

--

### `replacing(_ substring: String, with newString: String)`
String by replacing part of string with another string.
 - **type**: Method
 - **return type**: String
 - **parameters**:
   - **substring**: old substring to find and replace
   - **newString**: new string to insert in old string place
 - **returns**: string after replacing substring with newString
 - **availability**: `iOS 8+` `tvOS 9+`
 - **unit tests**: `iOS`

Example
```swift
"%number% items".replacing("%number%", with "10") -> "10 items"
```