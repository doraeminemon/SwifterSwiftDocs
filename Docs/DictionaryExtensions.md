# Dictionary extensions


## Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`has(key: Key)`**](#haskey-key) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`jsonData(prettify: Bool)`**](#jsondataprettify-bool--false) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`jsonString(prettify: Bool)`**](#jsonstringprettify-bool--false) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`lowercaseAllKeys()`**](#lowercaseallkeys) | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |


--


## `has(key: Key)`
Check if key exists in dictionary.

 - **type**: Method.
 - **return type**: Bool
 - **parameters**:
  - **key**: key to search for.
 - **returns**: true if key exists in dictionary.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
let dict: [String : Any] = ["testKey": "testValue", "testArrayKey": [1, 2, 3, 4, 5]]
dict.has(key: "testKey") -> true
dict.has(key: "anotherKey") -> false
```


--


## `jsonData(prettify: Bool = false)`
JSON Data from dictionary.

 - **type**: Method.
 - **return type**: Data?
 - **parameters**:
  - **prettify**: set true to prettify data (default is false).
 - **returns**: optional JSON Data (if applicable).
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


--


## `jsonString(prettify: Bool = false)`
JSON Data from dictionary.

 - **type**: Method.
 - **return type**: String?
 - **parameters**:
  - **prettify**: set true to prettify string (default is false).
 - **returns**: optional JSON String (if applicable).
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
dict.jsonString() -> "{"testKey":"testValue","testArrayKey":[1,2,3,4,5]}"

dict.jsonString()
/*
returns the following string:

"{
  "testKey" : "testValue",
  "testArrayKey" : [
    1,
    2,
    3,
    4,
    5
  ]
}"

*/
```


--


## `lowercaseAllKeys()`
Lowercase all keys in dictionary.

 - **type**: Mutating Method.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
var dict = ["tEstKeY": "value"]
dict.lowercaseAllKeys()
print(dict) // prints "["testkey": "value"]"
```


--
