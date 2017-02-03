# UICollectionView Extensions

### Properties:
|Name | Description |
|:--- | :--- |
|**indexPathForLastItem**| Index path of last item in collectionView. |
|**lastSection**| Index of last section in collectionView. |
|**numberOfItems**| Number of all items in all sections of collectionView. |


### Methods:
|Name | Return | Description |
|:--- | :--- | :--- |
|**indexPathForLastItem(inSection section: Int)**| IndexPath? | IndexPath for last item in section. |
|**reloadData(_ completion: () -> Void)**| -- | Reload data with a completion handler. |
