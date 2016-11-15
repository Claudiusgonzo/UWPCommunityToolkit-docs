---
permalink: /en-US/api/Microsoft_Toolkit_Uwp_Services_Facebook_FacebookService.htm
title: Microsoft.Toolkit.Uwp.Services.Facebook.FacebookService API 
description: API page for Microsoft.Toolkit.Uwp.Services.Facebook.FacebookService
keywords: windows, app, toolkit, UWP, API
layout: api
search.product: eADQiWindows 10XVcnh
---


# FacebookService class

Class for connecting to Facebook.

## Members

The **FacebookService** class has the following types of members:

### Constructors

#### contructor

Initializes a new instance of the [FacebookService](Microsoft_Toolkit_Uwp_Services_Facebook_FacebookService.htm) class. Default private constructor.



### Methods

#### Initialize(System.String appId,Microsoft.Toolkit.Uwp.Services.Facebook.FacebookPermissions requiredPermissions,System.String windowsStoreId)

Initialize underlying provider with relevent token information.

##### Parameters



| Name | Description | Type |


#### PostToFeedWithDialogAsync(System.String title,System.String description,System.String link,System.String pictureUrl)

Enables posting data to the timeline using Facebook dialog.

##### Parameters



| Name | Description | Type |


#### ProcessResultsAsync(System.Collections.Generic.IReadOnlyList(System.Object) results,System.Int32 maxRecords)

Helper method to process pages of results from underlying service instance.

##### Parameters



| Name | Description | Type |


#### Initialize(Microsoft.Toolkit.Uwp.Services.Facebook.FacebookOAuthTokens oAuthTokens,Microsoft.Toolkit.Uwp.Services.Facebook.FacebookPermissions requiredPermissions)

Initialize underlying provider with relevent token information.

##### Parameters



| Name | Description | Type |


#### PostPictureToFeedAsync(System.String title,System.String pictureName,Windows.Storage.Streams.IRandomAccessStreamWithContentType pictureStream)

Enables posting a picture to the timeline

##### Parameters



| Name | Description | Type |


#### PostToFeedAsync(System.String title,System.String message,System.String description,System.String link,System.String pictureUrl)

Enables direct posting data to the timeline.

##### Parameters



| Name | Description | Type |


#### GetUserPictureInfoAsync()

Returns the [FacebookPicture](Microsoft_Toolkit_Uwp_Services_Facebook_FacebookPicture.htm) object associated with the logged user

##### Parameters



| Name | Description | Type |


#### LoginAsync()

Login with set of required requiredPermissions.

##### Parameters



| Name | Description | Type |


#### LogoutAsync()

Log out of the underlying service instance.

##### Parameters



| Name | Description | Type |


#### RequestAsync(Microsoft.Toolkit.Uwp.Services.Facebook.FacebookDataConfig config,System.Int32 maxRecords)

Request list data from service provider based upon a given config / query.

##### Parameters



| Name | Description | Type |


### Properties

#### LoggedUser

Gets the current logged user name.



#### WindowsStoreId

Gets a Windows Store ID associated with the current app



#### Instance

Gets public singleton property.



#### Provider

Gets a reference to an instance of the underlying data provider.



### Fields

#### paginatedArray

Reference to paginated array object for handling multiple pages of returned service list data.



#### instance

Private singleton field.



#### permissions

List of permissions required by the app.



#### queryResults

Strongly typed list of service query data.



#### isInitialized

Field for tracking initialization status.

