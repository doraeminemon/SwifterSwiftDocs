# UITableView Extensions

### Properties:
|Name | Description |
|:--- | :--- |
|**indexPathForLastRow**| Index path of last row in table. |
|**lastSection**| Index of last section in table. |
|**numberOfRows**| Number of all rows in all sections of table. |


### Methods:
|Name | Return | Description |
|:--- | :--- | :--- |
|**indexPathForLastRow(inSection section: Int)**| IndexPath? | IndexPath for last row in section. |
|**reloadData(_ completion: () -> Void)**| -- | Reload data with a completion handler. |
|**removeTableFooterView()**| -- | Remove TableFooterView. |
|**removeTableHeaderView()**| -- | Remove TableHeaderView. |
|**scrollToBottom(animated: Bool = true)**| -- | Scroll to bottom of TableView. |
|**scrollToTop(animated: Bool = true)**| -- | Scroll to top of TableView. |
