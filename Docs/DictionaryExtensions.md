# Dictionary extensions


## Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`has(key: Key)`**](#haskey-key) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`removeAll(keys: [Key])`**](#removeallkeys-key) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`jsonData(prettify: Bool)`**](#jsondataprettify-bool--false) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`jsonString(prettify: Bool)`**](#jsonstringprettify-bool--false) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`lowercaseAllKeys()`**](#lowercaseallkeys) | Mutating Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`+`**](#operator-) | Infix Operator | 8+ | 9+ | 3+ | 10.10+ |
| [**`-`**](#operator-) | Infix Operator | 8+ | 9+ | 3+ | 10.10+ |
| [**`+=`**](#operator--) | Infix Operator | 8+ | 9+ | 3+ | 10.10+ |
| [**`-=`**](#operator--) | Infix Operator | 8+ | 9+ | 3+ | 10.10+ |


---


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


---

## `removeAll(keys: [Key])`
Remove all keys of the dictionary.

 - **type**: Method.
 - **parameters**:
  - **keys**: keys to be removed.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
var dict : [String : String] = ["key1" : "value1", "key2" : "value2", "key3" : "value3"]
dict.removeAll(keys: ["key1", "key2"])
dict.keys.contains("key3") -> true
dict.keys.contains("key1") -> false
dict.keys.contains("key2") -> false
```


---


## `jsonData(prettify: Bool = false)`
JSON Data from dictionary.

 - **type**: Method.
 - **return type**: Data?
 - **parameters**:
  - **prettify**: set true to prettify data (default is false).
 - **returns**: optional JSON Data (if applicable).
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


---


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


---


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


---

---


## `Operator +`
Merge the keys/values of two dictionaries.

 - **type**: Infix Operator.
 - **return type**: [Key: Value]
 - **parameters**:
  - **lhs**: dictionary.
  - **rhs**: dictionary.
 - **returns**: A dictionary with keys and values from both.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
let dict : [String : String] = ["key1" : "value1"]
let dict2 : [String : String] = ["key2" : "value2"]
let result = dict + dict2
result["key1"] -> "value1"
result["key2"] -> "value2"
```


---


## `Operator -`
Remove contained in the array from the dictionary.

 - **type**: Infix Operator.
 - **return type**: [Key: Value]
 - **parameters**:
  - **lhs**: dictionary.
  - **rhs**: array with the keys to be removed.
 - **returns**: A new dictionary with keys removed.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
let dict : [String : String] = ["key1" : "value1", "key2" : "value2", "key3" : "value3"]
let result = dict-["key1", "key2"]
result.keys.contains("key3") -> true
result.keys.contains("key1") -> false
result.keys.contains("key2") -> false
```


---


## `Operator +=`
Append the keys and values from the second dictionary into the first one.

 - **type**: Infix Operator.
 - **parameters**:
  - **lhs**: dictionary.
  - **rhs**: dictionary.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
var dict : [String : String] = ["key1" : "value1"]
let dict2 : [String : String] = ["key2" : "value2"]
dict += dict2
dict["key1"] -> "value1"
dict["key2"] -> "value2"
```


---



## `Operator -=`
Remove contained in the array from the dictionary.

 - **type**: Infix Operator.
 - **parameters**:
  - **lhs**: dictionary.
  - **rhs**: array with the keys to be removed.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
var dict : [String : String] = ["key1" : "value1", "key2" : "value2", "key3" : "value3"]
dict-=["key1", "key2"]
dict.keys.contains("key3") -> true
dict.keys.contains("key1") -> false
dict.keys.contains("key2") -> false
```


---
