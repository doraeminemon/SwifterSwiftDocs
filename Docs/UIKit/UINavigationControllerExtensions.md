# UINavigationController Extensions

## Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`popViewController(completion: (()->Void)?)`**](#popviewcontrollercompletion--void--nil) | Method | 8+ | 9+ | - | - |
| [**`pushViewController(viewController: UIViewController, completion: (()->Void)?)`**](#pushviewcontrollerviewcontroller-uiviewcontroller-completion--void--nil) | Method | 8+ | 9+ | - | - |
| [**`makeTransparent(withTint: UIColor)`**](#maketransparentwithtint-uicolor--white) | Method | 8+ | 9+ | - | - |


---


## `popViewController(completion: (()->Void)? = nil)`
Pop ViewController with completion handler.

- **type**: Method.
- **parameters**:
    - **completion**: optional completion handler (default is nil).
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let navigationController = UINavigationController()
navigationController.popViewController()
navigationController.popViewController() {
    print("Completion: The view controller has been popped")
}
```


---


## `pushViewController(viewController: UIViewController, completion: (()->Void)? = nil)`
Push ViewController with completion handler.

- **type**: Method.
- **parameters**:
     - **viewController**: viewController to push.
    - **completion**: optional completion handler (default is nil).
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let navigationController = UINavigationController()
let viewController = UIViewController()
navigationController.pushViewController(viewController)
navigationController.pushViewController(viewController) {
    print("Completion: The view controller has been pushed")
}
```


---


## `makeTransparent(withTint: UIColor = .white)`
Make navigation controller's navigation bar transparent.

- **type**: Method.
- **parameters**:
    - **withTint**: tint color (default is .white).
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let navigationController = UINavigationController()
navigationController.makeTransparent()
navigationController.makeTransparent(withTint: .black)
```

---
