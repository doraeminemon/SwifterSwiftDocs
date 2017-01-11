# Documentations Contributing Guidelines

This document contains information and guidelines about contributing to the documentations of this project. Please read it before you start participating.


## Topics
- [Important Notes Before Adding Documentations](#importantnotesbeforeaddingdocumentations)
- [Extension Types](#extensiontypes)
- [Documentation Template](#documentationtemplate)
- [Releases Flow](#releasesflow)
- [Reporting Issues](#reportingissues)




## Important Notes Before Contributing
- All documentations should be written in Markdown and in a clear English, if you are not familiar with markdown please refer to [this great cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) by [Adam Pritchard](https://github.com/adam-p).
- Documentations are grouped in one file based on the Type they extend (e.g. All String extensions documentations are grouped in **StringExtensions.md** file).
- All doc files are added to the [Docs folder](https://github.com/SwifterSwift/SwifterSwiftDocs/tree/master/Docs).
- The first source for any extension is the original documentations found in the [Extensions directory](https://github.com/SwifterSwift/SwifterSwift/tree/stable/Source/Extensions) in [SwifterSwift repository](https://github.com/SwifterSwift/SwifterSwift), incase they have any mistake, please open a pull request to update it before adding documentations here.
- **DO NOT** put any personal data about you in the context, your name, email, website or what so ever. 
- Even if you are a team member **DO NOT** contribute to the repo directly, instead make a fork to your personal account, and send a pull request.

## Extension Types

### Enumerations
- Enumeration `enum`

### Properties
- Property `var`
- Read-Only Property `var`
- Static Property `static var`
- Static Read-Only Property `static var`

### Methods
- Method `func`
- Mutating Method `mutating func`
- Static Method `static func` `class func`

### Initializers
- Initializer `init`
- Optional Initializer `init?`

### Operators
- Prefix Operator
- Infix Operator
- Postfix Operator


## Documentation Template
Please refer to [this template](https://github.com/SwifterSwift/SwifterSwiftDocs/blob/master/Templates/ExtensionsTemplate.md) before adding new documentations with keeping in mind the following:

- The order of added documentations should be the same of their original places in the [SwifterSwift repository](https://github.com/SwifterSwift/SwifterSwift).
- Do not forget to add a **`.`** at the end of lines.
- Do not forget to add in-page link in the **Table of Contents** table for each extension to its line in the documentation file.

## Releases Flow
Changes are made to [master](https://github.com/SwifterSwift/SwifterSwiftDocs/tree/master) branch directly and merged into [stable](https://github.com/SwifterSwift/SwifterSwiftDocs/tree/stable) branch for every stable release.

All new documentations, updated documentations and accepted pull requests will be added to master branch
Pull requests from master will be created and merged into stable branch whenever there is a new stable release.


## Reporting Issues
A great way to contribute to the documentations is to send a detailed issue when you encounter an problem. We always appreciate a well-written, thorough report.

Check that the documentations issues database doesn't already include that problem before submitting an issue. If you find a match, add a quick "+1" or "I have this problem too". Doing this helps prioritize the most common problems and requests.
