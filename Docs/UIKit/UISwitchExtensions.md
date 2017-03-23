# UISwitch Extensions

## Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`toggle(animated: Bool)`**](#toggleanimated-bool--true) | Method | 8+ | - | - | - |


---


# `toggle(animated: Bool = true)`
Toggle a UISwitch

- **type**: Method
- **parameters**:
    - **animated**: set true to animate the change (default is true)
- **return type**: Void
- **availability**: `iOS 8+`.
- **unit tests**: `iOS`.

Example

```swift
let switch = UISwitch()
switch.toggle()
switch.toggle(animated: false)
```


---
