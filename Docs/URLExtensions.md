# URL Extensions


## Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`appendingQueryParameters(_ parameters: [String: String])`**](#appendingqueryparameters_-parameters-string-string) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`appendQueryParameters(_ parameters: [String: String])`**](#appendqueryparameters_-parameters-string-string) | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |


---


## `appendingQueryParameters(_ parameters: [String: String])`
URL with appending query parameters.

 - **type**: Method.
 - **return type**: URL
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
let url = URL(string: "https://google.com")!
let param = ["q": "Swifter Swift"]
let queryUrl = url.appendingQueryParameters(params) -> "https://google.com?q=Swifter%20Swift"
```


---


## `appendQueryParameters(_ parameters: [String: String])`
Append query parameters to URL.

 - **type**: Mutating Method.
 - **return type**: URL
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
var url = URL(string: "https://google.com")!
let param = ["q": "Swifter Swift"]
url.appendQueryParameters(params)
print(url) // prints "https://google.com?q=Swifter%20Swift"
```


---
