# NSAttributedString Extensions


## Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`bolded`**](#bolded) | Read-Only Property | 8+ | - | - | 10.10+ |
| [**`underlined`**](#underlined) | Read-Only Property | 8+ | 9+ | 3+ | 10.10+ |
| [**`italicized`**](#italicized) | Read-Only Property | 8+ | - | - | - |
| [**`struckthrough`**](#struckthrough) | Read-Only Property | 8+ | - | 3+ | 10.10+ |
| [**`colored(with color: UIColor/NSColor)`**](#coloredwith-color-uicolornscolor) | Method | 8+ | 9+ | 3+ | 10.10+ |
| [**`+=`**](#operator-) | Infix Operator | 8+ | 9+ | 3+ | 10.10+ |


--


## `bolded`
Bolded string.

 - **type**: Read-Only Property.
 - **return type**: NSAttributedString
 - **availability**: `iOS 8+` `macOS 10.10+`.


--


## `underlined`
Underlined string.

 - **type**: Read-Only Property.
 - **return type**: NSAttributedString
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.



## `italicized`
Italicized string.

 - **type**: Read-Only Property.
 - **return type**: NSAttributedString
 - **availability**: `iOS 8+`.


--



## `struckthrough`
Struckthrough string.

 - **type**: Read-Only Property.
 - **return type**: NSAttributedString
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


--


## `colored(with color: UIColor/NSColor)`
Add color to string.

 - **type**: Method.
 - **return type**: NSAttributedString
 - **parameters**:
  - **color**: text color (NSColor for mac, and UI color for other operating systems).
 - **returns**: a NSAttributedString versions of string colored with given color.
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


--

## `Operator +=`
Add a NSAttributedString to another NSAttributedString.

 - **type**: Infix Operator.
 - **return type**: NSAttributedString
 - **availability**: `iOS 8+` `tvOS 9+` `watchOS 3+` `macOS 10.10+`.


--
