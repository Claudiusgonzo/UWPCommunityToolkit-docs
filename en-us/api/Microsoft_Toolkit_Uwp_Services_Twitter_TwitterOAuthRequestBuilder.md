---
permalink: /en-US/api/Microsoft_Toolkit_Uwp_Services_Twitter_TwitterOAuthRequestBuilder.htm
title: Microsoft.Toolkit.Uwp.Services.Twitter.TwitterOAuthRequestBuilder API 
description: API page for Microsoft.Toolkit.Uwp.Services.Twitter.TwitterOAuthRequestBuilder
keywords: windows, app, toolkit, UWP, API
layout: api
search.product: eADQiWindows 10XVcnh
---


# TwitterOAuthRequestBuilder class

OAuth request builder.

## Members

The **TwitterOAuthRequestBuilder** class has this types of members

* [constructors](#constructors)

* [methods](#methods)

* [properties](#properties)

* [fields](#fields)

### constructors

#### contructor

Initializes a new instance of the [TwitterOAuthRequestBuilder](Microsoft_Toolkit_Uwp_Services_Twitter_TwitterOAuthRequestBuilder.htm) class. Authorization request builder.

##### parameters



| name | description | type |


### methods

#### GetAuthHeaderParameters()

Get list of auth header parameters.

##### parameters



| name | description | type |


#### GetEncodedUri(System.Uri requestUri,System.Collections.Generic.IEnumerable(Microsoft.Toolkit.Uwp.Services.OAuth.OAuthParameter) parameters)

Get encoded Uri.

##### parameters



| name | description | type |


#### GenerateNonce()

Generate nonce.

##### parameters



| name | description | type |


#### GenerateTimeStamp()

Generate timestamp string.

##### parameters



| name | description | type |


#### GenerateSignature()

Generate signature.

##### parameters



| name | description | type |


#### GenerateAuthorizationHeader()

Generate authorization header.

##### parameters



| name | description | type |


#### GetSignParameters()

Get list of sign parameters.

##### parameters



| name | description | type |


### properties

#### SignatureMethod

Gets signature method.



#### ConsumerKey

Gets consumer key.



#### ConsumerSecret

Gets consumer secret.



#### Verb

Gets or sets HTTP verb for request.



#### TokenSecret

Gets access token secret.



#### Signature

Gets signature getter.



#### AuthorizationHeader

Gets authorization header getter.



#### Token

Gets access token.



#### EncodedRequestUri

Gets encoded Request Uri.



#### RequestUriWithoutQuery

Gets request Uri without query.



#### QueryParams

Gets list of query parameters.



#### Version

Gets version.



#### Nonce

Gets nonce.



#### Timestamp

Gets timestamp.



### fields

#### Realm

Realm for request.

