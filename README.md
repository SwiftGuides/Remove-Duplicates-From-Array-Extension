# Remove-Duplicates-From-Array-Extension
This extension will remove duplicate values from array

```swift
//MARK: extension to remove duplictes
extension Array where Element:Equatable {
    func removeDuplicates() -> [Element] {
        var result = [Element]()
        
        for value in self {
            if result.contains(value) == false {
                result.append(value)
            }
        }
        
        return result
    }
}
```
