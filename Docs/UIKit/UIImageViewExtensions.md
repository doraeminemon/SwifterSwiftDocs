# UIImageView Extensions

## Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`download(from url: URL, contentMode: UIViewContentMode, placeholder: UIImage?, completionHandler: ((UIImage?) -> Void)?)`**](#downloadfrom-url-url-contentmode-uiviewcontentmode--scaleaspectfit-placeholder-uiimage--nil-completionhandler-uiimage---void--nil) | Method | 8+ | 9+ | - | - |
| [**`blur(withStyle style: UIBlurEffectStyle)`**](#blurwithstyle-style-uiblureffectstyle--light) | Method | 8+ | 9+ | - | - |
| [**`blurred(withStyle style: UIBlurEffectStyle)`**](#blurredwithstyle-style-uiblureffectstyle--light) | Method | 8+ | 9+ | - | - |


---


# `download(from url: URL, contentMode: UIViewContentMode = .scaleAspectFit, placeholder: UIImage? = nil, completionHandler: ((UIImage?) -> Void)? = nil)`
Set image from a URL.

- **type**: Method
- **parameters**:
    - **url**: URL of image.
    - **contentMode**: imageView content mode (default is .scaleAspectFit).
    - **placeholder**: optional placeholder image.
    - **completionHandler**: optional completion handler to run when download finishs (default is nil).
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let imageView = UIImageView()
let url = URL(string: https://github.com/SwifterSwift)!
let placeholder = UIImage()
imageView.download(from: url)
imageView.download(from: url, contentMode: .scaleAspectFill, placeholder: placeholder) { (image: UIImage?) in
    print("SwifterSwift: Image download has finished")
}
```


---


# `blur(withStyle style: UIBlurEffectStyle = .light)`
Make image view blurry.

- **type**: Method
- **parameters**:
    - **style**: UIBlurEffectStyle (default is .light).
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let imageView = UIImageView()
imageView.blur()
imageView.blur(withStyle: .dark)
```


---


# `blurred(withStyle style: UIBlurEffectStyle = .light)`
Blurred version of an image view.

- **type**: Method
- **parameters**:
    - **style**: UIBlurEffectStyle (default is .light).
- **returns**: blurred version of self.
- **return type**: UIImageView
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

```swift
let imageView = UIImageView()
let blurredImageView = imageView.blurred()
let darkBlurred = imageView.blur(withStyle: .dark)
```

---
