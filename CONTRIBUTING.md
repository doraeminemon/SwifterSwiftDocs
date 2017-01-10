# Documentations Contributing Guidelines

This document contains information and guidelines about contributing to the documentations of this project. Please read it before you start participating.


## Topics
- [Important Notes Before Adding Documentations](#importantnotesbeforeaddingdocumentations)
- [Extension Types](#extensiontypes)
- [Documentation Template](#documentationtemplate)
- [Releases Flow](#releasesflow)
- [Reporting Issues](#reportingissues)




## Important Notes Before Contributing
- All documentations should be written in Markdown, if you are not familiar with markdown please refer to [this great cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) by [Adam Pritchard](https://github.com/adam-p) 
- Documentations are grouped in one file based on the Type they extend (e.g. All String extensions documentations are grouped in **StringExtensions.md** file)  
- All doc files are added to the [Docs folder](https://github.com/SwifterSwift/SwifterSwiftDocs/tree/master/Docs)
- The origianl documentations for any extension (e.g. ) is the main source, incase it has any mistake, please open a pull request to update it before adding documentations here.


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


## Documentation Template
Please refer to [this template]() before adding new documentations


## Releases Flow
Changes are made to [master](https://github.com/SwifterSwift/SwifterSwiftDocs/tree/master) branch directly and merged into [stable](https://github.com/SwifterSwift/SwifterSwiftDocs/tree/stable) branch for every stable release.

All new documentations, updated documentations and accepted pull requests will be added to master branch
Pull requests from master will be created and merged into stable branch whenever there is a new stable release.


## Reporting Issues
A great way to contribute to the documentations is to send a detailed issue when you encounter an problem. We always appreciate a well-written, thorough report.

Check that the documentations issues database doesn't already include that problem before submitting an issue. If you find a match, add a quick "+1" or "I have this problem too". Doing this helps prioritize the most common problems and requests.