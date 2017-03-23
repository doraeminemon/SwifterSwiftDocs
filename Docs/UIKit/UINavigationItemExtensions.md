# UINavigationItem Extensions

## Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`replaceTitle(with image: UIImage)`**](#replacetitlewith-image-uiimage) | Method | 8+ | 9+ | - | - |


--


## `replaceTitle(with image: UIImage)`
Replace title label with an image in navigation item.

- **type**: Method.
- **parameters**:
    - **image**: UIImage to replace title with.
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let navigationItem = UINavigationItem()
let image = UIImage()
navigationItem.replaceTitle(with: image)
```
