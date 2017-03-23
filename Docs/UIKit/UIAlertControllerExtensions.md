# UIAlertController Extensions

## Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`show(animated: Bool, vibrate: Bool, completion: (() -> Void)?)`**](#showanimated-bool--true-vibrate-bool--false-completion----void--nil) | Method | 8+ | - | - | - |
| [**`addAction(title: String, style: UIAlertActionStyle, isEnabled: Bool, handler: ((UIAlertAction) -> Void)?)`**](#addactiontitle-string-style-uialertactionstyle--default-isenabled-bool--true-handler-uialertaction---void--nil) | Method | 8+ | - | - | - |
| [**`addTextField(text: String?, placeholder: String?, editingChangedTarget: Any?, editingChangedSelector: Selector?)`**](#addtextfieldtext-string--nil-placeholder-string--nil-editingchangedtarget-any-editingchangedselector-selector) | Method | 8+ | - | - | - |
| [**`init(title: String, message: String?, defaultActionButtonTitle: String, tintColor: UIColor?)`**](#inittitle-string-message-string--nil-defaultactionbuttontitle-string--ok-tintcolor-uicolor--nil) | Initializer | 8+ | - | - | - |
| [**`init(title: String, error: Error, defaultActionButtonTitle: String, tintColor: UIColor?)`**](#inittitle-string--error-error-error-defaultactionbuttontitle-string--ok-tintcolor-uicolor--nil) | Initializer | 8+ | - | - | - |

--


## `show(animated: Bool = true, vibrate: Bool = false, completion: (() -> Void)? = nil)`
Present alert view controller in the current view controller.

- **type**: Method.
- **parameters**:
    - **animated**: set true to animate presentation of alert controller (default is true).
    - **vibrate**: set true to vibrate the device while presenting the alert (default is false).
    - **completion**: an optional completion handler to be called after presenting alert controller (default is nil).
- **return type**: Void
- **availability**: `iOS 8+`.
- **unit tests**: `iOS`.

Example

```swift
UIAlertController().show()
UIAlertController().show(animated: true, vibrate: false, completion: nil)
```


--

## `addAction(title: String, style: UIAlertActionStyle = .default, isEnabled: Bool = true, handler: ((UIAlertAction) -> Void)? = nil)`
Add an action to Alert

- **type**: Method.
- **parameters**:
    - **title**: action title.
    - **style**: action style (default is UIAlertActionStyle.default)
    - **isEnabled**: isEnabled status for action (default is true)
    - **handler**: optional action handler to be called when button is tapped (default is nil)
- **return type**: UIAlertAction (discardable result)
- **availability**: `iOS 8+`.
- **unit tests**: `iOS`.


Example

```swift
let alertActionDefault = UIAlertController().addAction(title: "Title")
let alertAction = UIAlertController().addAction(title: "Title", style: .default, isEnabled: true, handler: nil)
```

--

## `addTextField(text: String? = nil, placeholder: String? = nil, editingChangedTarget: Any?, editingChangedSelector: Selector?)`
Add a text field to Alert

- **type**: Method.
- **parameters**:
    - **text**: text field text (default is nil)
    - **placeholder**: text field placeholder text (default is nil)
    - **editingChangedTarget**: an optional target for text field's editingChanged
    - **editingChangedSelector**: an optional selector for text field's editingChanged
- **return type**: Void
- **availability**: `iOS 8+`.
- **unit tests**: `iOS`.


Example

```swift
UIAlertController().addTextField(editingChangedTarget: nil, editingChangedSelector: nil)
UIAlertController().addTextField(text: "Text", placeHolder: "PlaceHolder", editingChangedTarget: nil, editingChangedSelector: nil)
```

--

## `init(title: String, message: String? = nil, defaultActionButtonTitle: String = "OK", tintColor: UIColor? = nil)`
Create new alert view controller with default OK action.

- **type**: Initializer.
- **parameters**:
    - **title**: alert controller's title.
    - **message**: alert controller's message (default is nil).
    - **defaultActionButtonTitle**: default action button title (default is "OK")
    - **tintColor**: alert controller's tint color (default is nil)
- **return type**: UIAlertController
- **availability**: `iOS 8+`.
- **unit tests**: `iOS`.


Example

```swift
let alertDefault = UIAlertController(title: "Title")
let alert = UIAlertController(title: "Title", message: "Message", defaultActionButtleTitle: "No", tintColor: .black)
```

--

## `init(title: String = "Error", error: Error, defaultActionButtonTitle: String = "OK", tintColor: UIColor? = nil)`
Create new error alert view controller from Error with default OK action.

- **type**: Initializer.
- **parameters**:
    - **title**: alert controller's title (default is "Error").
    - **message**: error to set alert controller's message to it's localizedDescription.
    - **defaultActionButtonTitle**: default action button title (default is "OK")
    - **tintColor**: alert controller's tint color (default is nil)
- **return type**: UIAlertController
- **availability**: `iOS 8+`.
- **unit tests**: `iOS`.


Example

```swift
let alertDefault = UIAlertController(error: Error())
let alert = UIAlertController(title: "Title", error: Error(), defaultActionButtonTitle: "Ok", tintColor: .green)
```

--

