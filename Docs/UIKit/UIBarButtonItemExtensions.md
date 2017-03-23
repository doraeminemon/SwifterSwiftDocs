# UIBarButtonItem Extensions

## Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`addTargetForAction(target: AnyObject, action: Selector)`**](#addtargetforactiontarget-anyobject-action-selector) | Method | 8+ | 9+ | - | - |


---


## `addTargetForAction(target: AnyObject, action: Selector)`
Add Target to UIBarButtonItem

- **type**: Method.
- **parameters**:
    - **target**: target.
    - **action**: selector to run when button is tapped.
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
UIBarButtonItem().addTargetForAction(target: UIViewController(), action: #selector(UIViewController.barButtonAction))
```


---
