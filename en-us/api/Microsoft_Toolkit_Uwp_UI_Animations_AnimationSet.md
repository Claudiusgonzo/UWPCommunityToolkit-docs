---
permalink: /en-US/api/Microsoft_Toolkit_Uwp_UI_Animations_AnimationSet.htm
title: Microsoft.Toolkit.Uwp.UI.Animations.AnimationSet API 
description: API page for Microsoft.Toolkit.Uwp.UI.Animations.AnimationSet
keywords: windows, app, toolkit, UWP, API
layout: api
search.product: eADQiWindows 10XVcnh
---


# AnimationSet class

Defines an object for storing and managing CompositionAnimations for an element

## Members

The **AnimationSet** class has the following types of members:

### Constructors

#### contructor

Initializes a new instance of the [AnimationSet](Microsoft_Toolkit_Uwp_UI_Animations_AnimationSet.htm) class.

##### Parameters



| Name | Description | Type |


### Methods

#### SetDurationForAll(System.TimeSpan duration)

Ovewrites the duration on all animations to the specified value

##### Parameters



| Name | Description | Type |


#### Dispose()

Dispose resources.



#### AddEffectDirectPropertyChange(Windows.UI.Composition.CompositionEffectBrush effectBrush,System.Single value,System.String propertyName)

Adds an effect propety change to be run on StartAsync

##### Parameters



| Name | Description | Type |


#### AddStoryboardAnimation(System.String propertyPath,Windows.UI.Xaml.Media.Animation.Timeline timeline)

Adds a storyboard animation to be run

##### Parameters



| Name | Description | Type |


#### Start()

Stats all animations. This method is not awaitable.



#### StartAsync()

Starts all animations and returns an awaitable task.

##### Parameters



| Name | Description | Type |


#### Stop()

Stops all animations.



#### Then()

Wait for existing animations to complete before running new animations

##### Parameters



| Name | Description | Type |


#### SetDuration(System.Double duration)

Ovewrites the duration on all animations after last Then() to the specified value

##### Parameters



| Name | Description | Type |


#### SetDuration(System.TimeSpan duration)

Ovewrites the duration on all animations after last Then() to the specified value

##### Parameters



| Name | Description | Type |


#### SetDurationForAll(System.Double duration)

Ovewrites the duration on all animations to the specified value

##### Parameters



| Name | Description | Type |


#### RemoveCompositionDirectPropertyChange(System.String propertyName)

Removes a composition property change

##### Parameters



| Name | Description | Type |


#### SetDelay(System.Double delayTime)

Ovewrites the delay time on all animations after last Then() to the specified value

##### Parameters



| Name | Description | Type |


#### SetDelay(System.TimeSpan delayTime)

Ovewrites the delay time on all animations after last Then() to the specified value

##### Parameters



| Name | Description | Type |


#### SetDelayForAll(System.Double delayTime)

Ovewrites the delay time on all animations to the specified value

##### Parameters



| Name | Description | Type |


#### SetDelayForAll(System.TimeSpan delayTime)

Ovewrites the delay time on all animations to the specified value

##### Parameters



| Name | Description | Type |


#### AddCompositionAnimation(System.String propertyName,Windows.UI.Composition.CompositionAnimation animation)

Adds a composition animation to be run on StartAsync

##### Parameters



| Name | Description | Type |


#### RemoveCompositionAnimation(System.String propertyName)

Removes a composition animation from being run on Visual property

##### Parameters



| Name | Description | Type |


#### AddCompositionEffectAnimation(Windows.UI.Composition.CompositionEffectBrush effectBrush,Windows.UI.Composition.CompositionAnimation animation,System.String propertyName)

Adds a composition effect animation to be run on backing Visual

##### Parameters



| Name | Description | Type |


#### AddCompositionDirectPropertyChange(System.String propertyName,System.Object value)

Adds a composition property that will change instantaneously

##### Parameters



| Name | Description | Type |


### Properties

#### Visual

Gets the Visual object that backs the XAML element



#### Element

Gets the [UIElement](https://msdn.microsoft.com/library/windows/apps/Windows.UI.Xaml.UIElement)



#### UseComposition

Gets or sets a value indicating whether composition must be use even on SDK > 10586



### Events

#### Completed

Occurs when all animations have completed

