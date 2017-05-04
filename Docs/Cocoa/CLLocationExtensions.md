# CLLocation Extensions


## Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`midLocation(start: CLLocation, end: CLLocation) -> CLLocation`**](#midlocationstart-cllocation-end-cllocation---cllocation) | Class Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`midLocation(to point: CLLocation) -> CLLocation`**](#midlocationto-point-cllocation---cllocation) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`bearing(to destination: CLLocation) -> Double`**](#bearingto-destination-cllocation---double) | Method | 8+ | 9+ | 3+ | 10.10+ |


---


## `midLocation(start: CLLocation, end: CLLocation) -> CLLocation`
Calculate the half-way point along a great circle path between the two points.

 - **type**: Class Method.
 - **parameters**:
  - **start**: Start location.
  - **end**: End location.
 - **return type**: CLLocation
 - **returns**: Location that represents the half-way point.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
let a = CLLocation(latitude: -15.822877, longitude: -47.941839)
let b = CLLocation(latitude: -15.692030, longitude: -47.594397)
CLLocation.midLocation(start: a, end: b) -> CLLocation: -15.7575223324019, -47.7680620274339
```


---


## `midLocation(to point: CLLocation) -> CLLocation`
Calculate the half-way point along a great circle path between self and another points.

 - **type**: Method.
 - **parameters**:
  - **point**: End location.
 - **return type**: CLLocation
 - **returns**: Location that represents the half-way point.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
let a = CLLocation(latitude: -15.822877, longitude: -47.941839)
let b = CLLocation(latitude: -15.692030, longitude: -47.594397)
a.midLocation(to: b) -> CLLocation: -15.7575223324019, -47.7680620274339
```


---


## `bearing(to destination: CLLocation) -> Double`
Calculates the bearing to another CLLocation.

 - **type**: Method.
 - **parameters**:
  - **destination**: Location to calculate bearing.
 - **return type**: Double
 - **returns**: Calculated bearing degrees in the range 0° ... 360°
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.

Example

```swift
let a = CLLocation(latitude: -15.822877, longitude: -47.941839)
let b = CLLocation(latitude: -15.692030, longitude: -47.594397)
a.bearing(to: b) -> 105.619
```


---
