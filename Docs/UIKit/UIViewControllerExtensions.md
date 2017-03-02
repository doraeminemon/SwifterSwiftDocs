# UIViewController Extensions

##Table of Contents
| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`isVisible`**](#isvisible) | Read-Only Property | 8+ | 9+ | - | - |
| [**`navigationBar`**](#navigationbar) | Read-Only Property | 8+ | 9+ | - | - |
| [**`addNotificationObserver(name: Notification.Name, selector: Selector)`**](#addnotificationobservername-notificationname-selector-selector) | Method | 8+ | 9+ | - | - |
| [**`removeNotificationObserver(name: Notification.Name)`**](#removenotificationobservername-notificationname) | Method | 8+ | 9+ | - | - |
| [**`removeNotificationsObserver()`**](#removenotificationsobserver) | Method | 8+ | 9+ | - | - |

--

# `isVisible`
Check if ViewController is onscreen and not hidden.

- **type**: Property.
- **return type**: Bool
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let viewController = UIViewController()
let visibility = viewController.isVisible
```

--

# `navigationBar`
NavigationBar in a ViewController.

- **type**: Property.
- **return type**: UINavigationBar
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let viewController = UIViewController()
let navBar = viewController.navigationBar
```

--

# `addNotificationObserver(name: Notification.Name, selector: Selector)`
Assign as listener to notification.

- **type**: Method
- **parameters**:
    - **name**: notification name.
    - **selector**: selector to run with notified.
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let viewController = UIViewController()
let notification = Notification.Name("SwifterSwift")
viewController.addNotificationObserver(name: notification)
```

--

# `removeNotificationObserver(name: Notification.Name)`
Unassign as listener to notification.

- **type**: Method
- **parameters**:
    - **name**: notification name.
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let viewController = UIViewController()
let notification = Notification.Name("SwifterSwift")
viewController.removeNotificationObserver(name: notification)
```

--

# `removeNotificationsObserver()`
Unassign as listener from all notifications.

- **type**: Method
- **parameters**:
    - **name**: notification name.
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let viewController = UIViewController()
viewController.removeNotificationsObserver()
```

