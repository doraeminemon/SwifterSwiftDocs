# Collection Extensions


### Methods:
|Name | Return | Description |
|:--- | :--- | :--- |
|**forEachInParallel(_ each: (Self.Iterator.Element) -> ())**| -- | performs `each` closure for each element of collection in parallel. |
|**subscript (safe index: Index)**| Generator.Element? | Safe protects the array from out of bounds by use of optional. |
