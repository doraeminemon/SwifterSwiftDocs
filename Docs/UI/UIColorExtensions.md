# UIColor Extensions

### Properties:
|Name | Description |
|:--- | :--- |
|**complementary**| Get color complementary (read-only, if applicable). |
|**redComponent**| Red component of UIColor (read-only). |
|**greenComponent**| Green component of UIColor (read-only). |
|**blueComponent**| blue component of UIColor (read-only). |
|**alpha**| Alpha of UIColor (read-only). |
|**hexString**| Hexadecimal value string (read-only). |
|**shortHexString**| Short hexadecimal value string (read-only, if applicable). |
|**shortHexOrHexString**| Short hexadecimal value string, or full hexadecimal string if not possible (read-only). |
|**random**| Random color. |

### Methods:
|Name | Return | Description |
|:--- | :--- | :--- |
|**blend(_ color1: UIColor, intensity1: CGFloat = 0.5, with color2: UIColor, intensity2: CGFloat = 0.5)**| UIColor | Blend two UIColors |


### Initializers:
|Name | Description |
|:--- | :--- |
|**init(hex: Int, transparency: CGFloat = 1)**| Create UIColor from hexadecimal value with optional transparency. |
|**init(red: Int, green: Int, blue: Int, transparency: CGFloat = 1)**| Create UIColor from RGB values with optional transparency. |
|**init?(hexString: String, transparency: CGFloat)**| Create UIColor from hexadecimal string with optional transparency (if applicable). |
|**init?(complementaryFor color: UIColor)**| Create UIColor from a complementary of a UIColor (if applicable). |


### Structs:
|Name | Description |
|:--- | :--- |
|**social**| Brand identity color of popular social media platform. |
|**material**| Material colors |
|**css**| CSS colors |
