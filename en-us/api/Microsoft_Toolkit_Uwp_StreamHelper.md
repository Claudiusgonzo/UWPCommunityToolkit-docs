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

The **StreamHelper** class has the following types of members:

### Methods

#### IsPackagedFileExistsAsync(System.String fileName)

Test if a file exists in the application installation folder.

##### Parameters



| Name | Description | Type |


#### GetHttpStreamAsync(System.Uri uri)

Get the response stream returned by a HTTP get request.

##### Parameters



| Name | Description | Type |


#### GetPackagedFileStreamAsync(System.String fileName,Windows.Storage.FileAccessMode accessMode)

Return a stream to a specified file from the installation folder.

##### Parameters



| Name | Description | Type |


#### GetLocalFileStreamAsync(System.String fileName,Windows.Storage.FileAccessMode accessMode)

Return a stream to a specified file from the application local folder.

##### Parameters



| Name | Description | Type |


#### GetLocalCacheFileStreamAsync(System.String fileName,Windows.Storage.FileAccessMode accessMode)

Return a stream to a specified file from the application local cache folder.

##### Parameters



| Name | Description | Type |


#### GetKnowFoldersFileStreamAsync(Windows.Storage.KnownFolderId knownFolderId,System.String fileName,Windows.Storage.FileAccessMode accessMode)

Return a stream to a specified file from the application local cache folder.

##### Parameters



| Name | Description | Type |


#### GetHttpStreamToStorageFileAsync(System.Uri uri,Windows.Storage.StorageFile targetFile)

Get the response stream returned by a HTTP get request and save it to a local file.

##### Parameters



| Name | Description | Type |


#### IsLocalFileExistsAsync(System.String fileName)

Test if a file exists in the application local folder.

##### Parameters



| Name | Description | Type |


#### IsLocalCacheFileExistsAsync(System.String fileName)

Test if a file exists in the application local cache folder.

##### Parameters



| Name | Description | Type |


#### IsKnownFolderFileExistsAsync(Windows.Storage.KnownFolderId knownFolderId,System.String fileName)

Test if a file exists in the application local cache folder.

##### Parameters



| Name | Description | Type |


#### IsFileExistsAsync(Windows.Storage.StorageFolder workingFolder,System.String fileName)

Test if a file exists in the application local folder.

##### Parameters



| Name | Description | Type |


#### ReadTextAsync(Windows.Storage.Streams.IRandomAccessStream stream,System.Text.Encoding encoding)

Read stream content as a string.

##### Parameters



| Name | Description | Type |
