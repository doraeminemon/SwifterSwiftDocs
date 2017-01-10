# SwifterSwiftDocs

## Table of Contents
- [Requirements](#requirements)
- [Installation](#installation)
- [List of All Extensions](#listofallextensions)
- [How to contribute to the documentations](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/stable/CONTRIBUTING.md)
- [How to contribute to the project](https://github.com/SwifterSwift/SwifterSwift/blob/stable/CONTRIBUTING.md)


## Requirements:
- iOS 8.0+ / tvOS 9.0+
- Xcode 8.1+
- Swift 3.0+

SwifterSwift is for both iOS and tvOS, however most of the extensions should work on watchOS, and macOS.

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


### List of All Extensions