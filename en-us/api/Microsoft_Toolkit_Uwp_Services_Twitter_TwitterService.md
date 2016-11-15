---
permalink: /en-US/api/Microsoft_Toolkit_Uwp_Services_Twitter_TwitterService.htm
title: Microsoft.Toolkit.Uwp.Services.Twitter.TwitterService API 
description: API page for Microsoft.Toolkit.Uwp.Services.Twitter.TwitterService
keywords: windows, app, toolkit, UWP, API
layout: api
search.product: eADQiWindows 10XVcnh
---


# TwitterService class

Class for connecting to Twitter.

## Members

The **TwitterService** class has the following types of members:

### Constructors

#### contructor

Initializes a new instance of the [TwitterService](Microsoft_Toolkit_Uwp_Services_Twitter_TwitterService.htm) class. Default private constructor.



### Methods

#### Initialize(Microsoft.Toolkit.Uwp.Services.Twitter.TwitterOAuthTokens oAuthTokens)

Initialize underlying provider with relevent token information.

##### Parameters



| Name | Description | Type |


#### Logout()

Log user out of Twitter.



#### TweetStatusAsync(System.String message,Windows.Storage.Streams.IRandomAccessStream[] pictures)

Post a Tweet with associated pictures.

##### Parameters



| Name | Description | Type |


#### LoginAsync()

Log user in to Twitter.

##### Parameters



| Name | Description | Type |


#### RequestAsync(Microsoft.Toolkit.Uwp.Services.Twitter.TwitterDataConfig config,System.Int32 maxRecords)

Request list data from service provider based upon a given config / query.

##### Parameters



| Name | Description | Type |


#### GetUserTimeLineAsync(System.String screenName,System.Int32 maxRecords)

Retrieve user timeline data.

##### Parameters



| Name | Description | Type |


#### Initialize(System.String consumerKey,System.String consumerSecret,System.String callbackUri)

Initialize underlying provider with relevent token information.

##### Parameters



| Name | Description | Type |


#### GetUserAsync(System.String screenName)

Retrieve user data.

##### Parameters



| Name | Description | Type |


#### SearchAsync(System.String hashTag,System.Int32 maxRecords)

Search for specific hash tag.

##### Parameters



| Name | Description | Type |


### Properties

#### Provider

Gets a reference to an instance of the underlying data provider.



#### UserScreenName

Gets the current logged in user screen name.



#### Instance

Gets public singleton property.



### Fields

#### tokens

Field for tracking oAuthTokens.



#### instance

Private singleton field.



#### isInitialized

Field for tracking initialization status.



#### twitterDataProvider

Private singleton field for TwitterDataProvider.

