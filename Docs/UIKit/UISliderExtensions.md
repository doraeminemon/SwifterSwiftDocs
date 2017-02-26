# UISlider Extensions

##Table of Contents
| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`setValue(_ value: Float, animated: Bool, duration: TimeInterval, completion: (() -> Void)?)`**](#setvalue_-value-float-animated-bool--true-duration-timeinterval--1-completion----void--nil) | Method | 8+ | - | - | - |

--

## `setValue(_ value: Float, animated: Bool = true, duration: TimeInterval = 1, completion: (() -> Void)? = nil)`
Set slide bar value with completion handler.

- **type**: Method.
- **parameters**:
    - **value**: slider value.
    - **animated**: set true to animate value change (default is true).
    - **duration**: animation duration in seconds (default is 1 second).
    - **completion**: an optional completion handler to run after value is changed (default is nil)
- **return type**: Void
- **availability**: `iOS 8+`.
- **unit tests**: `iOS`.

Example

```swift
let slider = UISlider()
slider.minimumValue = 0
slider.maximumValue = 100
slider.setValue(99)
slider.setValue(17, animated: false, duration: 2)
```
