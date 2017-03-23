# UITabBar Extensions

## Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`setColors(background: UIColor?, selectedBackground: UIColor?, item: UIColor?, selectedItem: UIColor?)`**](#setcolorsbackground-uicolor--nil-selectedbackground-uicolor--nil-item-uicolor--nil-selecteditem-uicolor--nil) | Method | 8+ | 9+ | - | - |

--

# `setColors(background: UIColor? = nil, selectedBackground: UIColor? = nil, item: UIColor? = nil, selectedItem: UIColor? = nil)`
Set tabBar colors.

- **type**: Method
- **parameters**:
    - **background**: background color.
    - **selectedBackground**: background color for selected tab.
    - **item**: icon tint color for items.
    - **selectedItem**: icon tint color for item.
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.

Example

```swift
let tabBar = UITabBar()
tabBar.setColors()
tabBar.setColors(background: .red, selectedBackground: .blue, item: .yellow, selectedItem: .green)
```
