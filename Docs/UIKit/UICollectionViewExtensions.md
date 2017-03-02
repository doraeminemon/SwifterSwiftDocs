# UICollectionView Extensions

##Table of Contents
| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`indexPathForLastItem`**](#indexpathforlastitem) | Read-Only Property | 8+ | 9+ | - | - |
| [**`lastSection`**](#lastsection) | Read-Only Property | 8+ | 9+ | - | - |
| [**`numberOfItems`**](#numberofitems) | Read-Only Property | 8+ | 9+ | - | - |
| [**`indexPathForLastItem(inSection section: Int)`**](#indexpathforlastiteminsection-section-int) | Method | 8+ | 9+ | - | - |
| [**`reloadData(_ completion: () -> Void)`**](#reloaddata_-completion----void) | Method | 8+ | 9+ | - | - |
| [**`dequeReusableCell <T: UICollectionViewCell> (withClass name: T.Type, for indexPath: IndexPath)`**](#dequereusablecell-t-uicollectionviewcell-withclass-name-ttype-for-indexpath-indexpath) | Method | 8+ | 9+ | - | - |
| [**`dequeReusableSupplementaryView <T: UICollectionReusableView> (ofKind: String, withClass name: T.Type, for indexPath: IndexPath)`**](#dequereusablesupplementaryview-t-uicollectionreusableview-ofkind-string-withclass-name-ttype-for-indexpath-indexpath) | Method | 8+ | 9+ | - | - |
| [**`register <T: UICollectionReusableView> (supplementaryViewOfKind kind: String, withClass name: T.Type)`**](#register-t-uicollectionreusableview-supplementaryviewofkind-kind-string-withclass-name-ttype) | Method | 8+ | 9+ | - | - |
| [**`register <T: UICollectionViewCell> (nib: UINib?, forCellWithClass name: T.Type)`**](#register-t-uicollectionviewcell-nib-uinib-forcellwithclass-name-ttype) | Method | 8+ | 9+ | - | - |
| [**`register <T: UICollectionViewCell> (cellWithClass name: T.Type)`**](#register-t-uicollectionviewcell-cellwithclass-name-ttype) | Method | 8+ | 9+ | - | - |
| [**`register <T: UICollectionReusableView> (nib: UINib?, forSupplementaryViewOfKind kind: String, withClass name: T.Type)`**](#register-t-uicollectionreusableview-nib-uinib-forsupplementaryviewofkind-kind-string-withclass-name-ttype) | Method | 8+ | 9+ | - | - |

--

# `indexPathForLastItem`
Index path of last item in collectionView.

- **type**: Property.
- **return type**: IndexPath
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let collectionView = UICollectionView()
let indexPath = collectionView.indexPathForLastItem
```

--

# `lastSection`
Index of last section in collectionView.

- **type**: Property.
- **return type**: Int
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let collectionView = UICollectionView()
let lastSection = collectionView.lastSection
```

--

# `numberOfItems`
Number of all items in all sections of collectionView.

- **type**: Property.
- **return type**: Int
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let collectionView = UICollectionView()
let itemCount = collectionView.numberOfItems
```

--

# `indexPathForLastItem(inSection section: Int)`
IndexPath for last item in section.

- **type**: Method
- **parameters**:
    - **section**: section to get last item in.
- **return type**: IndexPath?
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let collectionView = UICollectionView()
let indexPath = collectionView.indexPathForLastItem(section: 0)
```

--

# `reloadData(_ completion: () -> Void)`
Reload data with a completion handler.

- **type**: Method
- **parameters**:
    - **completion**: completion handler to run after reloadData finishes.
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.

Example

```swift
let collectionView = UICollectionView()
collectionView.reloadData {
   print("SwifterSwift: Data has completed reloading")
}
```

--

# `dequeReusableCell <T: UICollectionViewCell> (withClass name: T.Type, for indexPath: IndexPath)`
Deque reusable UICollectionViewCell using class name.

- **type**: Method
- **parameters**:
    - **name**: UICollectionViewCell type.
    - **indexPath**: Location of cell in collectionView.
- **returns**: UICollectionViewCell object with associated class name.
- **return type**: T (must be type of UICollectionViewCell)
- **availability**: `iOS 8+`, `tvOS 9+`.

Example

```swift
let collectionView = UICollectionView()
let indexPath = IndexPath()
let cell = collectionView.dequeReusableCell(withClass: UICollectionViewCell.self, for: indexPath)
```

--

# `dequeReusableSupplementaryView <T: UICollectionReusableView> (ofKind: String, withClass name: T.Type, for indexPath: IndexPath)`
Deque reusable UICollectionReusableView using class name.

- **type**: Method
- **parameters**:
    - **ofKind**: The kind of supplementary view to retrieve. This value is defined by the layout object.
    - **name**: UICollectionReusableView type.
    - **indexPath**: Location of cell in collectionView.
- **returns**: UICollectionReusableView object with associated class name.
- **return type**: T (must be type of UICollectionReusableView)
- **availability**: `iOS 8+`, `tvOS 9+`.

Example

```swift
let collectionView = UICollectionView()
let indexPath = IndexPath()
let reusableView = collectionView.dequeReusableSupplementaryView(ofKind: "UICollectionReusableView", withClass: UICollectionReusableView.self, for: indexPath)
```

--

# `register <T: UICollectionReusableView> (supplementaryViewOfKind kind: String, withClass name: T.Type)`
Register UICollectionReusableView using class name.

- **type**: Method
- **parameters**:
    - **kind**: The kind of supplementary view to retrieve. This value is defined by the layout object.
    - **name**: UICollectionReusableView type
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.

Example

```swift
let collectionView = UICollectionView()
collectionView.register(supplementaryViewOfKind: "UICollectionReusableView", withClass: UICollectionReusableView.self)
```

--

# `register <T: UICollectionViewCell> (nib: UINib?, forCellWithClass name: T.Type)`
Register UICollectionViewCell using class name.

- **type**: Method
- **parameters**:
    - **nib**: Nib file used to create the collectionView cell.
    - **name**: UICollectionViewCell type.
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.

Example

```swift
let collectionView = UICollectionView()
let nib = UINib()
collectionView.register(nib: nib, forCellWithClass: UICollectionViewCell.self)
```

--

# `register <T: UICollectionViewCell> (cellWithClass name: T.Type)`
Register UICollectionViewCell using class name.

- **type**: Method
- **parameters**:
    - **name**: UICollectionViewCell type.
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.

Example

```swift
let collectionView = UICollectionView()
collectionView.register(cellWithClass: UICollectionViewCell.self)
```

--

# `register <T: UICollectionReusableView> (nib: UINib?, forSupplementaryViewOfKind kind: String, withClass name: T.Type)`
Register UICollectionReusableView using class name.

- **type**: Method
- **parameters**:
    - **nib**: Nib file used to create the reusable view.
    - **kind**: The kind of supplementary view to retrieve. This value is defined by the layout object.
    - **name**: UICollectionReusableView type.
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.

Example

```swift
let collectionView = UICollectionView()
let nib = UINib()
collectionView.register(nib: nib, forSupplementaryViewOfKind: "UICollectionReusableView", withClass: UICollectionReusableView.self)
```


