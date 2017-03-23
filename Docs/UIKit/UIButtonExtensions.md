# UIButton Extensions

## Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`imageForDisabled`**](#imagefordisabled) | Property | 8+ | 9+ | - | - |
| [**`imageForHighlighted`**](#imageforhighlighted) | Property | 8+ | 9+ | - | - |
| [**`imageForNormal`**](#imagefornormal) | Property | 8+ | 9+ | - | - |
| [**`imageForSelected`**](#imageforselected) | Property | 8+ | 9+ | - | - |
| [**`titleColorForDisabled`**](#titlecolorfordisabled) | Property | 8+ | 9+ | - | - |
| [**`titleColorForHighlighted`**](#titlecolorforhighlighted) | Property | 8+ | 9+ | - | - |
| [**`titleColorForNormal`**](#titlecolorfornormal) | Property | 8+ | 9+ | - | - |
| [**`titleColorForSelected`**](#titlecolorforselected) | Property | 8+ | 9+ | - | - |
| [**`titleForDisabled`**](#titlefordisabled) | Property | 8+ | 9+ | - | - |
| [**`titleForHighlighted`**](#titleforhighlighted) | Property | 8+ | 9+ | - | - |
| [**`titleForNormal`**](#titlefornormal) | Property | 8+ | 9+ | - | - |
| [**`titleForSelected`**](#titleforselected) | Property | 8+ | 9+ | - | - |
| [**`setImageForAllStates(_ image: UIImage)`**](#setimageforallstates_-image-uiimage) | Method | 8+ | 9+ | - | - |
| [**`setTitleColorForAllStates(_ color: UIColor)`**](#settitlecolorforallstates_-color-uicolor) | Method | 8+ | 9+ | - | - |
| [**`setTitleForAllStates(_ title: String)`**](#settitleforallstates_-title-string) | Method | 8+ | 9+ | - | - |


---


## `imageForDisabled`
Image of disabled state for button; also inspectable from Storyboard.

- **type**: Property.
- **return type**: UIImage?
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let button = UIButton()
let imageForDisabled = button.imageForDisabled
button.imageForDisabled = UIImage()
```


---


## `imageForHighlighted`
Image of highlighted state for button; also inspectable from Storyboard.

- **type**: Property.
- **return type**: UIImage?
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let button = UIButton()
let imageForHighlighted = button.imageForHighlighted
button.imageForHighlighted = UIImage()
```


---


## `imageForNormal`
Image of normal state for button; also inspectable from Storyboard.

- **type**: Property.
- **return type**: UIImage?
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let button = UIButton()
let imageForNormal = button.imageForNormal
button.imageForNormal = UIImage()
```


---


## `imageForSelected`
Image of selected state for button; also inspectable from Storyboard.

- **type**: Property.
- **return type**: UIImage?
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let button = UIButton()
let imageForSelected = button.imageForSelected
button.imageForSelected = UIImage()
```


---


## `titleColorForDisabled`
Title color of disabled state for button; also inspectable from Storyboard.

- **type**: Property.
- **return type**: UIColor?
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let button = UIButton()
let titleColorForDisabled = button.titleColorForDisabled
button.titleColorForDisabled = .blue
```


---


## `titleColorForHighlighted`
Title color of highlighted state for button; also inspectable from Storyboard.

- **type**: Property.
- **return type**: UIColor?
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let button = UIButton()
let titleColorForHighlighted = button.titleColorForHighlighted
button.titleColorForHighlighted = .blue
```

---


## `titleColorForNormal`
Title color of normal state for button; also inspectable from Storyboard.

- **type**: Property.
- **return type**: UIColor?
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let button = UIButton()
let titleColorForNormal = button.titleColorForNormal
button.titleColorForNormal = .blue
```


---


## `titleColorForSelected`
Title color of selected state for button; also inspectable from Storyboard.

- **type**: Property.
- **return type**: UIColor?
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let button = UIButton()
let titleColorForSelected = button.titleColorForSelected
button.titleColorForSelected = .blue
```


---


## `titleForDisabled`
Title of disabled state for button; also inspectable from Storyboard.

- **type**: Property.
- **return type**: String?
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let button = UIButton()
let titleForDisabled = button.titleForDisabled
button.titleColorForDisabled = "New Title"
```


---


## `titleForHighlighted`
Title of highlighted state for button; also inspectable from Storyboard.

- **type**: Property.
- **return type**: String?
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let button = UIButton()
let titleForHighlighted = button.titleForHighlighted
button.titleForHighlighted = "New Title"
```


---


## `titleForNormal`
Title of normal state for button; also inspectable from Storyboard.

- **type**: Property.
- **return type**: String?
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let button = UIButton()
let titleForNormal = button.titleForNormal
button.titleForNormal = "New Title"
```


---


## `titleForSelected`
Title of selected state for button; also inspectable from Storyboard.

- **type**: Property.
- **return type**: String?
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let button = UIButton()
let titleForSelected = button.titleForSelected
button.titleForSelected = "New Title"
```


---


## `setImageForAllStates(_ image: UIImage)`
Set image for all states.

- **type**: Method
- **parameters**:
    - **image**: UIImage.
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let button = UIButton()
let image = UIImage()
button.setImageForAllStates(image)
```


---


## `setTitleColorForAllStates(_ color: UIColor)`
Set title color for all states.

- **type**: Method
- **parameters**:
    - **color**: UIColor.
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let button = UIButton()
button.setTitleColorForAllStates(.green)
```


---


## `setTitleForAllStates(_ title: String)`
Set title for all states.

- **type**: Method
- **parameters**:
    - **title**: title String.
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let button = UIButton()
button.setTitleForAllStates("SwifterSwift")
```


---
