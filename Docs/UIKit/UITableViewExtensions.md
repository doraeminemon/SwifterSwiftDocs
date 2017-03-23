# UITableView Extensions

## Table of Contents

| Name | Type | iOS | tvOS | watchOS | macOS |
|:--- | :--- | :---: | :---: | :---: | :---: |
| [**`indexPathForLastRow`**](#indexpathforlastrow) | Read-Only Property | 8+ | 9+ | - | - |
| [**`lastSection`**](#lastsection) | Read-Only Property | 8+ | 9+ | - | - |
| [**`numberOfRows`**](#numberofrows) | Read-Only Property | 8+ | 9+ | - | - |
| [**`indexPathForLastItem(inSection section: Int)`**](#indexpathforlastrowinsection-section-int) | Method | 8+ | 9+ | - | - |
| [**`reloadData(_ completion: () -> Void)`**](#reloaddata_-completion----void) | Method | 8+ | 9+ | - | - |
| [**`removeTableFooterView()`**](#removetablefooterview) | Method | 8+ | 9+ | - | - |
| [**`removeTableHeaderView()`**](#removetableheaderview) | Method | 8+ | 9+ | - | - |
| [**`scrollToBottom()`**](#scrolltobottomanimated-bool--true) | Method | 8+ | 9+ | - | - |
| [**`scrollToTop()`**](#scrolltotopanimated-bool--true) | Method | 8+ | 9+ | - | - |
| [**`dequeueReusableCell <T: UITableViewCell> (withClass name: T.Type)`**](#dequeuereusablecell-t-uitableviewcell-withclass-name-ttype) | Method | 8+ | 9+ | - | - |
| [**`dequeueReusableCell <T: UITableViewCell> (withClass name: T.Type, for indexPath: IndexPath)`**](#dequeuereusablecell-t-uitableviewcell-withclass-name-ttype-for-indexpath-indexpath) | Method | 8+ | 9+ | - | - |
| [**`dequeueReusableHeaderFooterView <T: UITableViewHeaderFooterView> (withClass name: T.Type)`**](#dequeuereusableheaderfooterview-t-uitableviewheaderfooterview-withclass-name-ttype) | Method | 8+ | 9+ | - | - |
| [**`register <T: UITableViewHeaderFooterView> (nib: UINib?, withHeaderFooterViewClass name: T.Type)`**](#register-t-uitableviewheaderfooterview-nib-uinib-withheaderfooterviewclass-name-ttype) | Method | 8+ | 9+ | - | - |
| [**`register <T: UITableViewHeaderFooterView> (headerFooterViewClassWith name: T.Type)`**](#register-t-uitableviewheaderfooterview-headerfooterviewclasswith-name-ttype) | Method | 8+ | 9+ | - | - |
| [**`register <T: UITableViewCell> (cellWithClass name: T.Type)`**](#register-t-uitableviewcell-cellwithclass-name-ttype) | Method | 8+ | 9+ | - | - |
| [**`register <T: UITableViewCell> (nib: UINib?, withCellClass name: T.Type)`**](#register-t-uitableviewcell-nib-uinib-withcellclass-name-ttype) | Method | 8+ | 9+ | - | - |

--

# `indexPathForLastRow`
Index path of last row in tableView.

- **type**: Read-Only Property.
- **return type**: IndexPath?
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let tableView = UITableView()
let indexPath = tableView.indexPathForLastRow
```

--

# `lastSection`
Index of last section in tableView.

- **type**: Read-Only Property.
- **return type**: Int
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let tableView = UITableView()
let lastSection = tableView.lastSection
```

--

# `numberOfRows`
Number of all rows in all sections of tableView.

- **type**: Read-Only Property.
- **return type**: Int
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let tableView = UITableView()
let rowCount = tableView.numberOfRows
```

--

# `indexPathForLastRow(inSection section: Int)`
IndexPath for last row in section.

- **type**: Method
- **parameters**:
    - **section**: section to get last row in.
- **returns**: optional last indexPath for last row in section (if applicable).
- **return type**: IndexPath?
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let tableView = UITableView()
let indexPath = tableView.indexPathForLastRow(inSection: 0)
```

--

# `reloadData(_ completion: () -> Void)`
Reload data with a completion handler.

- **type**: Method
- **parameters**:
    - **completion**: completion handler to run after reloadData finishes.
- **return type**: Void.
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let tableView = UITableView()
tableView.reloadData {
    print("SwifterSwift: Reloading complete!")
}
```

--

# `removeTableFooterView()`
Remove TableFooterView.

- **type**: Method
- **return type**: Void.
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let tableView = UITableView()
tableView.removeTableFooterView()
```

--

# `removeTableHeaderView()`
Remove TableHeaderView.

- **type**: Method
- **return type**: Void.
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let tableView = UITableView()
tableView.removeTableHeaderView()
```

--

# `scrollToBottom(animated: Bool = true)`
Scroll to bottom of TableView.

- **type**: Method
- **parameter**:
    - **animated**: set true to animate scroll (default is true).
- **return type**: Void.
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let tableView = UITableView()
tableView.scrollToBottom()
tableView.scrollToBottom(animated: false)
```

--

# `scrollToTop(animated: Bool = true)`
Scroll to top of TableView.

- **type**: Method
- **parameter**:
    - **animated**: set true to animate scroll (default is true).
- **return type**: Void.
- **availability**: `iOS 8+`, `tvOS 9+`.
- **unit tests**: `iOS`, `tvOS`.

Example

```swift
let tableView = UITableView()
tableView.scrollToTop()
tableView.scrollToTop(animated: false)
```

--

# `dequeueReusableCell <T: UITableViewCell> (withClass name: T.Type)`
Dequeue reusable UITableViewCell using class name.

- **type**: Method
- **parameters**:
    - **name**: UITableViewCell type.
- **returns**: UITableViewCell object with associated class name (optional value).
- **return type**: T? (must be of type UITableViewCell)
- **availability**: `iOS 8+`, `tvOS 9+`.

Example

```swift
let tableView = UITableView()
let cell = tableView.dequeueReusableCell(withClass: UITableViewCell.self)
```

--

# `dequeueReusableCell <T: UITableViewCell> (withClass name: T.Type, for indexPath: IndexPath)`
Dequeue reusable UITableViewCell using class name for indexPath.

- **type**: Method
- **parameters**:
    - **name**: UITableViewCell type.
    - **indexPath**: UITableViewCell object with associated class name
- **returns**: UITableViewCell object with associated class name (optional value).
- **return type**: T (must be of type UITableViewCell)
- **availability**: `iOS 8+`, `tvOS 9+`.

Example

```swift
let tableView = UITableView()
let indexPath = IndexPath()
let cell = tableView.dequeueReusableCell(withClass: UITableViewCell.self, for: indexPath)
```

--

# `dequeueReusableHeaderFooterView <T: UITableViewHeaderFooterView> (withClass name: T.Type)`
Dequeue reusable UITableViewHeaderFooterView using class name.

- **type**: Method
- **parameters**:
    - **name**: UITableViewHeaderFooterView type.
- **returns**: UITableViewHeaderFooterView object with associated class name (optional value).
- **return type**: T? (must be of type UITableViewHeaderFooterView)
- **availability**: `iOS 8+`, `tvOS 9+`.

Example

```swift
let tableView = UITableView()
let headerFooterView = tableView.dequeueReusableHeaderFooterView(withClass: UITableViewHeaderFooterView.self)
```

--

# `register <T: UITableViewHeaderFooterView> (nib: UINib?, withHeaderFooterViewClass name: T.Type)`
Register UITableViewHeaderFooterView using class name.

- **type**: Method
- **parameters**:
    - **nib**: Nib file used to create the header or footer view.
    - **name**: UITableViewHeaderFooterView type.
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.

Example

```swift
let tableView = UITableView()
let nib = UINib()
tableView.register(nib: nib, withHeaderFooterViewClass: UITableViewHeaderFooterView.self)
```

--

# `register <T: UITableViewHeaderFooterView> (headerFooterViewClassWith name: T.Type)`
Register UITableViewHeaderFooterView using class name.

- **type**: Method
- **parameters**:
    - **name**: UITableViewHeaderFooterView type.
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.

Example

```swift
let tableView = UITableView()
let nib = UINib()
tableView.register(nib: nib, withHeaderFooterViewClass: UITableViewHeaderFooterView.self)
```

--

# `register <T: UITableViewCell> (cellWithClass name: T.Type)`
Register UITableViewCell using class name.

- **type**: Method
- **parameters**:
    - **name**: UITableViewCell type.
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.

Example

```swift
let tableView = UITableView()
tableView.register(cellWithClass: UITableViewCell.self)
```

--

# `register <T: UITableViewCell> (nib: UINib?, withCellClass name: T.Type)`
Register UITableViewCell using class name.

- **type**: Method
- **parameters**:
    - **nib**: Nib file used to create the tableView cell.
    - **name**: UITableViewCell type.
- **return type**: Void
- **availability**: `iOS 8+`, `tvOS 9+`.

Example

```swift
let tableView = UITableView()
let nib = UINib()
tableView.register(nib: nib, withCellClass: UITableViewCell.self)
```

--




