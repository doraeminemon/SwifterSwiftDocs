# UIImage Extensions

### Properties:

|Name | Description |
|:--- | :--- |
|**bytesSize**| Size in bytes of UIImage |
|**kilobytesSize**| Size in kilo bytes of UIImage |


### Methods:

|Name | Return | Description |
|:--- | :--- | :--- |
|**compressed(quality: CGFloat = 0.5)**| UIImage? | Compressed UIImage from original UIImage. |
|**compressedData(quality: CGFloat = 0.5)**| Data? | Compressed UIImage data from original UIImage. |
|**cropped(to rect: CGRect)**| UIImage | UIImage Cropped to CGRect. |
|**scaled(toHeight: CGFloat, with orientation: UIImageOrientation? = nil)**| UIImage? | UIImage scaled to height with respect to aspect ratio. |
|**scaled(toWidth: CGFloat, with orientation: UIImageOrientation? = nil)**| UIImage? | UIImage scaled to width with respect to aspect ratio. |
|**filled(withColor color: UIColor)**| UIImage | UIImage filled with color |


### Initializers:

|Name | Description |
|:--- | :--- |
|**init(color: UIColor, size: CGSize)**| Create UIImage from color and size. |
