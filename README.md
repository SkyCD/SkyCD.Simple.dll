# SkyCD.Simple.dll

[![GitHub release](https://img.shields.io/github/release/SkyCD/SkyCD.Simple.dll.svg)](https://github.com/SkyCD/SkyCD.Simple.dll/releases/latest)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://github.com/SkyCD/SkyCD.Simple.dll/blob/master/LICENSE)

SkyCD.Simple.dll is a library to provide structures to handle internal SkyCD items data.

## Classes

### Public Class skycd_simple

- Public Enum scdItemType As Byte
- Public Structure scdItem
- Public Items(0) As scdItem
- Private col As New Collection
- Public Function Add(ByVal Name As String, Optional ByVal ItemType As scdItemType = scdItemType.scdUnknown, Optional ByVal ParentID As Integer = -1) As Integer
- Public Function Remove(ByVal ID As Integer) As Boolean
- Public Function Exists(ByVal Name As String, Optional ByVal ParentID As Integer = -1) As Integer
- Public Function AddPath(ByVal Path As String, Optional ByVal ParentID As Integer = -1, Optional ByVal FirstItemType As scdItemType = scdItemType.scdFile, Optional ByVal LastItemType As scdItemType = scdItemType.scdFile) As Integer
- Sub Clear()

### Imports SkyCD.AdvancedFunctions

### Public Class scdProperties

- Structure scdPropertyItem
- Private Items(0) As scdPropertyItem
- Public Property Item(ByVal Name As String) As Object

## License

SkyCD.Simple.dll is open source and released under the MIT License. Please see the [LICENSE](LICENSE) file for more information.

## Contribution

We welcome any contributions and feedback to help improve this library. Please feel free to open an issue or submit a pull request on the project's GitHub page.
