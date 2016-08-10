---
permalink: /en-US/api/Microsoft_Toolkit_Uwp_UI_ImageCache.htm
title: Microsoft.Toolkit.Uwp.UI.ImageCache API 
description: API page for Microsoft.Toolkit.Uwp.UI.ImageCache
keywords: windows, app, toolkit, UWP, API
layout: api
search.product: eADQiWindows 10XVcnh
---


# ImageCache class

Provides methods and tools to cache images in a temporary local folder

## Members

The **ImageCache** class has this types of members

* [methods](#methods)

* [properties](#properties)

### methods

#### ClearAsync(System.Nullable(System.TimeSpan) duration)

call this method to clear the entire cache.

##### parameters



| name | description | type |


#### GetFromCacheAsync(System.Uri uri)

Load a specific image from the cache. If the image is not in the cache, ImageCache will try to download and store it.

##### parameters



| name | description | type |


#### GetCacheFileName(System.Uri uri)

Gets the local cache file name associated with a specified Uri.

##### parameters



| name | description | type |


### properties

#### CacheDuration

Gets or sets the life duration of every cache entry.

