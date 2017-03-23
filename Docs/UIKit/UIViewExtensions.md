# UIView Extensions

### Enums:

|Name | Description |
|:--- | :--- |
|**ShakeDirection**| Shake directions of a view. |
|**AngleUnit**| Angle units. |
|**ShakeAnimationType**| Shake animations types. |

### Properties:

|Name | Description |
|:--- | :--- |
|**borderColor**| Border color of view; also inspectable from Storyboard. |
|**borderWidth**| Border width of view; also inspectable from Storyboard. |
|**cornerRadius**| Corner radius of view; also inspectable from Storyboard. |
|**firstResponder**| First responder. |
|**height**| Height of view. |
|**isRightToLeft**| Check if view is in RTL format. |
|**parentViewController**| Get view's parent view controller (if applicable). |
|**screenshot**| Take screenshot of view (if applicable). |
|**shadowColor**| Shadow color of view; also inspectable from Storyboard. |
|**shadowOffset**| Shadow offset of view; also inspectable from Storyboard. |
|**shadowOpacity**| Shadow opacity of view; also inspectable from Storyboard. |
|**shadowRadius**| Shadow radius of view; also inspectable from Storyboard. |
|**size**| Size of view. |
|**width**| Width of view. |


### Methods:

|Name | Return | Description |
|:--- | :--- | :--- |
|**roundCorners(_ corners: UIRectCorner, radius: CGFloat)**| -- | Set some or all corners radiuses of view. |
|**addShadow(ofColor color: UIColor, radius: CGFloat,offset: CGSize, opacity: Float)**| -- | Add shadow to view. |
|**add(subViews: [UIView])**| -- | Add array of subviews to view. |
|**fadeIn(duration: TimeInterval, completion:((Bool) -> Void)?)**| -- | Fade in view. |
|**fadeOut(duration: TimeInterval, completion:((Bool) -> Void)?)**| -- | Fade out view. |
|**loadFromNib(named: String, bundle : Bundle? = nil)**| UIView? | Load view from nib. |
|**removeSubViews()**| -- | Remove all subviews in view. |
|**removeGestureRecognizers()**| -- | Remove all gesture recognizers from view. |
|**rotate(byAngle angle : CGFloat, ofType type: AngleUnit, animated: Bool, duration: TimeInterval, completion:((Bool) -> Void)?)**| -- | Rotate view by angle on relative axis. |
|**rotate(toAngle angle: CGFloat, ofType type: AngleUnit, animated: Bool, duration: TimeInterval, completion:((Bool) -> Void)?)**| -- | Rotate view to angle on fixed axis. |
|**scale(by offset: CGPoint, animated: Bool, duration: TimeInterval, completion:((Bool) -> Void)?)**| -- | Scale view by offset. |
|**shake(direction: ShakeDirection, duration: TimeInterval, animationType: ShakeAnimationType, completion:(() -> Void)?)**| -- | Shake view. |
|**func addConstraints(withFormat: String, views: UIView...)**| -- | Add Visual Format constraints. |
|**func fillToSuperview()**| -- | Anchor all sides of the view into it's superview. |
|**func anchor(top: NSLayoutYAxisAnchor?, left: NSLayoutXAxisAnchor?, bottom: NSLayoutYAxisAnchor?, right: NSLayoutXAxisAnchor?, topConstant: CGFloat, leftConstant: CGFloat, bottomConstant: CGFloat, rightConstant: CGFloat, widthConstant: CGFloat, heightConstant: CGFloat)**| [NSLayoutConstraint] | Add anchors from any side of the current view into the specified anchors and returns the newly added constraints. |
|**func anchorCenterXToSuperview(withConstant: CGFloat = 0)**| -- | Anchor center X into current view's superview with a constant margin value. |
|**func anchorCenterYToSuperview(constant: CGFloat = 0)**| -- | Anchor center Y into current view's superview with a constant margin value. |
|**func anchorCenterSuperview()**| -- | Anchor center X and Y into current view's superview |
