# SwifterSwift (convenience extensions)


### Properties:

|Name | Description |
|:--- | :--- |
|**appDisplayName**| App's name (if applicable). |
|**appBundleID**| App's bundle ID (if applicable). |
|**statusBarHeight**| StatusBar height |
|**appBuild**| App current build number (if applicable). |
|**applicationIconBadgeNumber**| Application icon badge current number. |
|**appVersion**| App's current version (if applicable). |
|**batteryLevel**| Current battery level. |
|**currentDevice**| Shared instance of current device. |
|**screenHeight**| Screen height. |
|**screenWidth**| Screen width. |
|**deviceModel**| Current device model. |
|**deviceName**| Current device name. |
|**deviceOrientation**| Current orientation of device. |
|**isInDebuggingMode**| Check if app is running in debug mode. |
|**isInTestFlight**| Check if app is running in TestFlight mode. |
|**isMultitaskingSupported**| Check if multitasking is supported in current device. |
|**isNetworkActivityIndicatorVisible**| Current status bar network activity indicator state. |
|**isPad**| Check if device is iPad. |
|**isPhone**| Check if device is iPhone. |
|**isRegisteredForRemoteNotifications**| Check if device is registered for remote notifications for current app (read only). |
|**isRunningOnSimulator**| Check if application is running on simulator (read only). |
|**isStatusBarHidden**| Status bar visibility state. |
|**keyWindow**| Key window (read only, if applicable). |
|**mostTopViewController**| Most top view controller (if applicable). |
|**sharedApplication**| Shared instance UIApplication. |
|**statusBarStyle**| Current status bar style (if applicable). |
|**systemVersion**| System current version (read-only). |
|**userDefaults**| Shared instance of standard UserDefaults (read-only). |


### Methods:

|Name | Return | Description |
|:--- | :--- | :--- |
|**delay(milliseconds: Double, queue: DispatchQueue = .main, completion: @escaping ()-> Void)**| -- | Delay function or closure call. |
|**debounce(millisecondsDelay: Int, queue: DispatchQueue = .main, action: @escaping (()->()))**| ()->() | Debounce function or closure call. |
|**didTakeScreenShot(_ action: @escaping () -> ())**| -- | Called when user takes a screenshot |
|**object(forKey: String)**| Any? | Object from UserDefaults. |
|**string(forKey: String)**| String? | String from UserDefaults. |
|**integer(forKey: String)**| Int? | Integer from UserDefaults. |
|**double(forKey: String)**| Double? | Double from UserDefaults. |
|**data(forKey: String)**| Data? | Data from UserDefaults. |
|**bool(forKey: String)**| Bool? | Bool from UserDefaults. |
|**array(forKey: String)**| [Any]? | Array from UserDefaults. |
|**dictionary(forKey: String)**| [String: Any]? | Dictionary from UserDefaults. |
|**float(forKey: String)**| Float? | Float from UserDefaults. |
|**set(value: Any?, forKey: String)**| -- | Save an object to UserDefaults. |
|**typeName(for object: Any)**| String | Class name of object as string. |
