# UISegmentedControl Extensions

## Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`segmentTitles`**](#segmenttitles) | Property | 8+ | 9+ | - | - |
| [**`segmentImages`**](#segmentimages) | Property | 8+ | 9+ | - | - |


---


## `segmentTitles`
Segments titles.

- **type**: Property.
- **return type**: [String]
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let segmentedControl = UISegmentedControl()
let titles = segmentedControl.segmentTitles
segmentedControl.segmentTitles = ["Swifter", "Swift"]
```


---


## `segmentImages`
Segments images.

- **type**: Property.
- **return type**: [UIImage]
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let segmentedControl = UISegmentedControl()
let images = segmentedControl.segmentImages
segmentedControl.segmentImages = [UIImage(), UIImage()]
```


---
