# UILabel Extensions

##Table of Contents
| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`requiredHeight`**](#requiredheight) | Read-Only Property | 10+ | 10+ | - | - |

--

# `requiredHeight`
Required height for a label

- **type**: Read-Only Property.
- **return type**: CGFloat
- **availability**: `iOS 10+`, `tvOS 10+`.


Example

```swift
let label = UILabel(frame: CGRect(x: 0, y: 0, width: 40, height: 40))
let reqHeight = label.requiredHeight
```

