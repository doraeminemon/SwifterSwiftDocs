# Array Extensions


### Properties:
|Name | Description |
|:--- | :--- |
|**randomItem**| Random item from array. |
|**shuffled**| Shuffled version of array. |
|**average**| Average of all elements in array. |
|**sum**| Sum of all elements in array. |
|**withoutDuplicates**| Array with all duplicates removed from it. |


### Methods:
|Name | Return | Description |
|:--- | :--- | :--- |
|**item(at index: Int)**| Element? | Element at the given index if it exists. |
|**firstIndex <Item: Equatable> (of item: Item)**| Int? | First index of a given item in an array. |
|**lastIndex <Item: Equatable> (of item: Item)**| Int? | Last index of element in array. |
|**pop()**| Element? | Remove last element from array and return it. |
|**prepend(_ newElement: Element)**| -- | Insert an element at the beginning of array. |
|**push(_ newElement: Element)**| -- | Insert an element to the end of array. |
|**shuffle()**| -- | Shuffle array. |
|**contains(_ elements: [Element])**| Bool | Check if array contains an array of elements. |
|**indexes(of item: Element)**| [Int] | All indexes of specified item. |
|**removeAll(_ item: Element)**| -- | Remove all instances of an item from array. |
