# UIAlertController Extensions

### Methods:
|Name | Return | Description |
|:--- | :--- | :--- |
|**show(animated: Bool = true, vibrate: Bool = false, completion: (() -> Void)? = nil)**| -- | Present alert view controller in the current view controller. |
|**addAction(title: String, style: UIAlertActionStyle = .default, isEnabled: Bool = true, handler: ((UIAlertAction) -> Void)? = nil)**| UIAlertAction | Add an action to Alert |
|**addTextField(text: String? = nil, placeholder: String? = nil, editingChangedTarget: Any?, editingChangedSelector: Selector?)**| -- | Add a text field to Alert |


### Initializers:
|Name | Description |
|:--- | :--- |
|**init(title: String, message: String? = nil, defaultActionButtonTitle: String = "OK", tintColor: UIColor? = nil)**| Create new alert view controller with default OK action. |
|**init(title: String = "Error", error: Error, defaultActionButtonTitle: String = "OK", tintColor: UIColor? = nil)**| Create new error alert view controller from Error with default OK action. |
