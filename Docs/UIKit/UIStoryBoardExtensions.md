##Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`mainStoryboard`**](#mainstoryboard) | Read-Only Property | 10+ | 10+ | - | - |
| [**`instantiateViewController<T: UIViewController>(withClass name: T.Type)`**](#instantiateviewcontrolert-uiviewcontrollerwithclass-name-ttype) | Method | 8+ | 9+ | - | - |

--

# `mainStoryboard`
Get main storyboard for application.

- **type**: Read-Only Property.
- **return type**: UIStoryboard?
- **availability**: `iOS 10+`, `tvOS 10+`.

Example

```swift
let storyboard = UIStoryboard.main
```

--

# `instantiateViewController<T: UIViewController>(withClass name: T.Type)`
Instantiate a UIViewController using its class name.

- **type**: Method.
- **parameters**:
    - **name**: UIViewController type.
- **return type**: T (must be UIViewController)
- **returns**: The view controller corresponding to specified class name.
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS 8+`, `tvOS 9+`.

Example

```swift
let viewcontroller = UIStoryboard().instantiateViewController(withClass: UIViewController.self)
```
