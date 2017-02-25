# UINavigationBar Extensions

##Table of Contents
| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`setTitleFont(_ font: UIFont, color: UIColor)`**](#settitlefont_-font-uifont-color-uicolor--black) | Method | 8+ | 9+ | - | - |
| [**`makeTransparent(withTint: UIColor)`**](#maketransparentwithtint-uicolor--white) | Method | 8+ | 9+ | - | - |
| [**`setColors(background: UIColor, text: UIColor)`**](#setcolorsbackground-uicolor-text-uicolor) | Method | 8+ | 9+ | - | - |

--

# `setTitleFont(_ font: UIFont, color: UIColor = .black)`
Set Navigation Bar title, title color and font.

- **type**: Method
- **parameters**:
    - **font**: title font.
    - **color**: title text color (default is .black).
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let navigationBar = UINavigationBar()
let font = UIFont(name: "HelveticaNeue-UltraLight", size: 30)
navigationBar.setTitleFont(font)
navigationBar.setTitleFont(font, color: .green)
```

--

# `makeTransparent(withTint: UIColor = .white)`
Make navigation bar transparent.

- **type**: Method
- **parameters**:
    - **withTint**: tint color (default is .white).
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let navigationBar = UINavigationBar()
navigationBar.makeTransparent()
navigationBar.makeTransparent(withTint: .black)
```

--

# `setColors(background: UIColor, text: UIColor)`
Set navigationBar background and text colors.

- **type**: Method
- **parameters**:
    - **background**: backgound color.
    - **text**: text color.
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let navigationBar = UINavigationBar()
navigationBar.setColors(background: .blue, text: .red)
```
