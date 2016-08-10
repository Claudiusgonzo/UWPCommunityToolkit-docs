---
permalink: /en-US/api/Microsoft_Toolkit_Uwp_StreamHelper.htm
title: Microsoft.Toolkit.Uwp.StreamHelper API 
description: API page for Microsoft.Toolkit.Uwp.StreamHelper
keywords: windows, app, toolkit, UWP, API
layout: api
search.product: eADQiWindows 10XVcnh
---


# StreamHelper class

This class provides static helper methods for streams.

## Members

The **StreamHelper** class has this types of members

* [methods](#methods)

### methods

#### IsPackagedFileExistsAsync(System.String fileName)

Test if a file exists in the application installation folder.

##### parameters



| name | description | type |


#### GetHttpStreamAsync(System.Uri uri)

Get the response stream returned by a HTTP get request.

##### parameters



| name | description | type |


#### GetPackagedFileStreamAsync(System.String fileName,Windows.Storage.FileAccessMode accessMode)

Return a stream to a specified file from the installation folder.

##### parameters



| name | description | type |


#### GetLocalFileStreamAsync(System.String fileName,Windows.Storage.FileAccessMode accessMode)

Return a stream to a specified file from the application local folder.

##### parameters



| name | description | type |


#### GetLocalCacheFileStreamAsync(System.String fileName,Windows.Storage.FileAccessMode accessMode)

Return a stream to a specified file from the application local cache folder.

##### parameters



| name | description | type |


#### GetKnowFoldersFileStreamAsync(Windows.Storage.KnownFolderId knownFolderId,System.String fileName,Windows.Storage.FileAccessMode accessMode)

Return a stream to a specified file from the application local cache folder.

##### parameters



| name | description | type |


#### GetHttpStreamToStorageFileAsync(System.Uri uri,Windows.Storage.StorageFile targetFile)

Get the response stream returned by a HTTP get request and save it to a local file.

##### parameters



| name | description | type |


#### IsLocalFileExistsAsync(System.String fileName)

Test if a file exists in the application local folder.

##### parameters



| name | description | type |


#### IsLocalCacheFileExistsAsync(System.String fileName)

Test if a file exists in the application local cache folder.

##### parameters



| name | description | type |


#### IsKnownFolderFileExistsAsync(Windows.Storage.KnownFolderId knownFolderId,System.String fileName)

Test if a file exists in the application local cache folder.

##### parameters



| name | description | type |


#### IsFileExistsAsync(Windows.Storage.StorageFolder workingFolder,System.String fileName)

Test if a file exists in the application local folder.

##### parameters



| name | description | type |


#### ReadTextAsync(Windows.Storage.Streams.IRandomAccessStream stream,System.Text.Encoding encoding)

Read stream content as a string.

##### parameters



| name | description | type |
