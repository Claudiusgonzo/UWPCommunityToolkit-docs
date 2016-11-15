---
permalink: /en-US/api/Microsoft_Toolkit_Uwp_Services_Twitter_TwitterDataProvider.htm
title: Microsoft.Toolkit.Uwp.Services.Twitter.TwitterDataProvider API 
description: API page for Microsoft.Toolkit.Uwp.Services.Twitter.TwitterDataProvider
keywords: windows, app, toolkit, UWP, API
layout: api
search.product: eADQiWindows 10XVcnh
---


# TwitterDataProvider class

Data Provider for connecting to Twitter service.

## Members

The **TwitterDataProvider** class has the following types of members:

### Constructors

#### contructor

Initializes a new instance of the [TwitterDataProvider](Microsoft_Toolkit_Uwp_Services_Twitter_TwitterDataProvider.htm) class. Constructor.

##### Parameters



| Name | Description | Type |


### Methods

#### UploadPicture(Windows.Storage.Streams.IRandomAccessStream stream)

Publish a picture to Twitter user's medias.

##### Parameters



| Name | Description | Type |


#### GetTimeStamp()

Generate timestamp.

##### Parameters



| Name | Description | Type |


#### GetNonce()

Generate nonce.

##### Parameters



| Name | Description | Type |


#### ExchangeRequestTokenForAccessToken(System.String webAuthResultResponseData)

Extract and initialize access tokens.

##### Parameters



| Name | Description | Type |


#### GetSignature(System.String sigBaseString,System.String consumerSecretKey)

Generate request signature.

##### Parameters



| Name | Description | Type |


#### GetUserAsync(System.String screenName)

Retrieve user data.

##### Parameters



| Name | Description | Type |


#### GetUserTimeLineAsync``1(System.String screenName,System.Int32 maxRecords,Microsoft.Toolkit.Uwp.Services.IParser(TT0) parser)

Retrieve user timeline data with specific parser.

##### Parameters



| Name | Description | Type |


#### SearchAsync``1(System.String hashTag,System.Int32 maxRecords,Microsoft.Toolkit.Uwp.Services.IParser(TT0) parser)

Search for specific hash tag with specific parser.

##### Parameters



| Name | Description | Type |


#### LoginAsync()

Log user in to Twitter.

##### Parameters



| Name | Description | Type |


#### Logout()

Log user out of Twitter.



#### TweetStatus(System.String tweet,Windows.Storage.Streams.IRandomAccessStream[] pictures)

Tweets a status update.

##### Parameters



| Name | Description | Type |


#### GetSignatureBaseStringParams(System.String consumerKey,System.String nonce,System.String timeStamp,System.String additionalParameters)

Build signature base string.

##### Parameters



| Name | Description | Type |


#### GetDefaultParser(Microsoft.Toolkit.Uwp.Services.Twitter.TwitterDataConfig config)

Returns parser implementation for specified configuration.

##### Parameters



| Name | Description | Type |


#### GetDataAsync``1(Microsoft.Toolkit.Uwp.Services.Twitter.TwitterDataConfig config,System.Int32 maxRecords,Microsoft.Toolkit.Uwp.Services.IParser(TT0) parser)

Wrapper around REST API for making data request.

##### Parameters



| Name | Description | Type |


#### ValidateConfig(Microsoft.Toolkit.Uwp.Services.Twitter.TwitterDataConfig config)

Check validity of configuration.

##### Parameters



| Name | Description | Type |


#### ExtractTokenFromResponse(System.String getResponse,Microsoft.Toolkit.Uwp.Services.Twitter.TwitterOAuthTokenType tokenType)

Extract requested token from the REST API response string.

##### Parameters



| Name | Description | Type |


#### GetHomeTimeLineAsync``1(System.Int32 maxRecords,Microsoft.Toolkit.Uwp.Services.IParser(TT0) parser)

Get home time line data.

##### Parameters



| Name | Description | Type |


#### InitializeRequestAccessTokens(System.String twitterCallbackUrl)

Package up token request.

##### Parameters



| Name | Description | Type |


### Properties

#### LoggedIn

Gets a value indicating whether the provider is already logged in



#### UserScreenName

Gets or sets logged in user information.



### Fields

#### tokens

Base Url for service.



#### vault

Password vault used to store access tokens



#### BaseUrl

Base Url for service.

