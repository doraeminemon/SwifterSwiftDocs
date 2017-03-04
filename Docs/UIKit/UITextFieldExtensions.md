# UITextField Extensions

##Table of Contents
| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`isEmpty`**](#isempty) | Read-Only Property | 8+ | 9+ | - | - |
| [**`trimmedText`**](#trimmedtext) | Read-Only Property | 8+ | 9+ | - | - |
| [**`leftViewTintColor`**](#leftviewtintcolor) | Property | 8+ | 9+ | - | - |
| [**`rightViewTintColor`**](#rightviewtintcolor) | Property | 8+ | 9+ | - | - |
| [**`clear()`**](#clear) | Method | 8+ | 9+ | - | - |
| [**`setPlaceHolderTextColor(_ color: UIColor)`**](#setplaceholdertextcolor_-color-uicolor) | Method | 8+ | 9+ | - | - |

--

# `isEmpty`
Check if text field is empty.

- **type**: Read-Only Property.
- **return type**: Bool
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let textField = UITextField()
let bool = textField.isEmpty
```

--

# `trimmedText`
Return text with no spaces or new lines in beginning and end.

- **type**: Read-Only Property.
- **return type**: String?
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let textField = UITextField()
let output = textField.trimmedText
```

--

# `leftViewTintColor`
Left view tint color.

- **type**: Property.
- **return type**: UIColor?
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let textField = UITextField()
let currentColor = textField.leftViewTintColor
textField.leftViewTintColor = .red
```

--

# `rightViewTintColor`
Right view tint color.

- **type**: Property.
- **return type**: UIColor?
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let textField = UITextField()
let currentColor = textField.rightViewTintColor
textField.rightViewTintColor = .red
```

--

# `clear`
Clear text.

- **type**: Method.
- **return type**: Void.
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let textField = UITextField()
textField.clear()
```

--

# `setPlaceHolderTextColor(_ color: UIColor)`
Set placeholder text color.

- **type**: Method.
- **parameters**:
    - **color**: placeholder text color.
- **return type**: Void.
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let textField = UITextField()
textField.setPlaceHolderTextColor(.green)
```
