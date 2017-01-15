# SwifterSwiftDocs

## Table of Contents
- [Requirements](#requirements)
- [List of All Extensions](#list-of-all-extensions)
- [Installation](#installation)
- [How to contribute to the documentations](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/stable/CONTRIBUTING.md)
- [How to contribute to the project](https://github.com/SwifterSwift/SwifterSwift/blob/stable/CONTRIBUTING.md)

## Requirements:
- iOS 8.0+ / tvOS 9.0+ / watchOS 3.0+ / macOS 10.10+
- Xcode 8.1+
- Swift 3.0+

## List of All Extensions

### [Array Extensions](./Docs/ArrayExtensions.md)
### [Bool Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/BoolExtensions.md)
### [Character Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/CharacterExtensions.md)
### [Collection Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/CollectionExtensions.md)
### [Data Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/DataExtensions.md)
### [Date Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/DateExtensions.md)
### [Dictionary Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/DictionaryExtensions.md)
### [Double Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/DoubleExtensions.md)
### [Float Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/FloatExtensions.md)
### [Int Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/IntExtensions.md)
### [String Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/StringExtensions.md)
### [SwifterSwift](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/SwifterSwift.md)

## List of UI Extensions
### [CGFloat Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/CGFloatExtensions.md)
### [CGPoint Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/CGPointExtensions.md)
### [CGSize Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/CGSizeExtensions.md)
### [NSAttributedString Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/NSAttributedStringExtensions.md)
### [UIAlertController Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/UIAlertControllerExtensions.md)
### [UIBarButtonItem Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/UIBarButtonItemExtensions.md)
### [UIButton Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/UIButtonExtensions.md)
### [UICollectionView Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/UICollectionViewExtensions.md)
### [UIColor Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/UIColorExtensions.md)
### [UIImage Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/UIImageExtensions.md)
### [UIImageView Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/UIImageViewExtensions.md)
### [UILabel Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/UILabelExtensions.md)
### [UINavigationBar Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/UINavigationBarExtensions.md)
### [UINavigationController Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/UINavigationControllerExtensions.md)
### [UINavigationItem Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/UINavigationItemExtensions.md)
### [UISearchBar Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/UISearchBarExtensions.md)
### [UISegmentedControl Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/UISegmentedControlExtensions.md)
### [UISlider Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/UISliderExtensions.md)
### [UISwitch Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/UISwitchExtensions.md)
### [UITabBar Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/UITabBarExtensions.md)
### [UITableView Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/UITableViewExtensions.md)
### [UITextField Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/UITextFieldExtensions.md)
### [UITextView Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/UITextViewExtensions.md)
### [UIViewController Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/UIViewControllerExtensions.md)
### [UIView Extensions](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Docs/UIViewExtensions.md)


## Installation

### CocoaPods

[CocoaPods](http://cocoapods.org) is a dependency manager for Cocoa projects. You can install it with the following command:

```bash
$ gem install cocoapods
```

To integrate SwifterSwift into your Xcode project using CocoaPods, specify it in your `Podfile`:

```ruby
source 'https://github.com/CocoaPods/Specs.git'
platform :ios, '8.0'
use_frameworks!

target '<Your Target Name>' do
    pod 'SwifterSwift'
end
```

Then, run the following command:

```bash
$ pod install
```


### Carthage

[Carthage](https://github.com/Carthage/Carthage) is a decentralized dependency manager that builds your dependencies and provides you with binary frameworks.

You can install Carthage with [Homebrew](http://brew.sh/) using the following command:

```bash
$ brew update
$ brew install carthage
```

To integrate SwifterSwift into your Xcode project using Carthage, specify it in your `Cartfile`:

```ogdl
github "SwifterSwift/SwifterSwift" ~> 1.4
```

Run `carthage update` to build the framework and drag the built `SwifterSwift.framework` into your Xcode project.



### Swift Package Manager

You can use [The Swift Package Manager](https://swift.org/package-manager) to install `SwifterSwift` by adding the proper description to your `Package.swift` file:

```swift
import PackageDescription

let package = Package(
    name: "YOUR_PROJECT_NAME",
    targets: [],
    dependencies: [
        .Package(url: "https://github.com/SwifterSwift/SwifterSwift.git", versions: Version(1,4,0)..<Version(3, .max, .max)),
    ]
)
```

Note that the [Swift Package Manager](https://swift.org/package-manager) is still in early design and development, for more information checkout its [GitHub Page](https://github.com/apple/swift-package-manager)



### Manually

Add the [extensions](https://github.com/SwifterSwift/SwifterSwift/tree/stable/Source) folder to your Xcode project to use all extensions, or a specific extension.
