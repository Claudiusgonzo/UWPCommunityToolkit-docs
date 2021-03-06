---
permalink: /en-US/animations.htm
title: Animations using visual composition  
description: Animations allow you to implement specific XAML behaviors and apply visual composition to your application, such as Blur and Fade. You can also use code to chain animations together without using XAML.
keywords: windows, app, toolkit, animation behavior, XAML behavior, animation, composition 
layout: api
search.product: eADQiWindows 10XVcnh
lang: en-us
---

# Animations

UWP Community toolkit provides several tools to animate your UIElements.

You can use behaviors from within Blend for an editor experience, or you can decide to do it manually using code.

## Animation Styles and Documentation

| Link | 
| --- |
| [Blur]({{site.baseurl}}/{{page.lang}}/animations/blur.htm) | 
| [Fade]({{site.baseurl}}/{{page.lang}}/animations/fade.htm) | 
| [Offset]({{site.baseurl}}/{{page.lang}}/animations/offset.htm) |
| [Rotate]({{site.baseurl}}/{{page.lang}}/animations/rotate.htm) | 
| [Scale]({{site.baseurl}}/{{page.lang}}/animations/scale.htm) | 


## Behaviors

Behaviors are powerful tools for designers that can be defined in Blend:

{% highlight xml %}

    <interactivity:Interaction.Behaviors>
        <behaviors:Blur x:Name="BlurBehavior" 
           Value="10" 
           Duration="10" 
           Delay="0" 
           AutomaticallyStart="True"/>
    </interactivity:Interaction.Behaviors>

{% endhighlight %}

You can specify to start animation automatically upon loading (with AutomaticallyStart="True") or you can use code to do it manually.

## Animations using code only

For developers, the toolkit provides extensions for UIElement to match what can be done with behaviors.

So for instance if you want to blur an element, you only need to call this code:

{% highlight csharp %}

await ToolkitLogo.Blur(duration: 10, delay: 0, value: 10).StartAsync();       

{% endhighlight %}

### Async/await

Animations are asynchronous by essence.  You can await an animation if you start it with `StartAsync()`, but there is also a non-awaitable (but still asynchronous) version if you start it with `Start()`:

{% highlight csharp %}

await ToolkitLogo.Blur(duration: 10, delay: 0, value: 10).StartAsync();       
ToolkitLogo.Blur(duration: 10, delay: 0, value: 10).Start();

{% endhighlight %}

### Chaining animations

You can also chain animations thanks to the toolkit fluid API:

{% highlight csharp %}

await element.Rotate(value: 30f).Fade(value: 0.5).Blur(value: 2).StartAsync();

{% endhighlight %}

In this case the toolkit will trigger a rotation, a fade and a blur simultaneously.

If you want to start animations in a serial way, you can use `Then()`:

{% highlight csharp %}

await element.Rotate(value: 30f).Then().Fade(value: 0.5).Then().Blur(value: 2).StartAsync();

{% endhighlight %}

Every animation can have its own duration but there is a way to set it up for all animations at once:

{% highlight csharp %}

    var anim = element.Rotate(value: 30f).Fade(value: 0.5).Blur(value: 5);
    anim.SetDurationForAll(2);
    anim.StartAsync();

{% endhighlight %}

As animations are awaitable, it is easy to execute code after animations are completed.
If you do not want to await your animations, you can then use the Completed event:

{% highlight csharp %}

    var anim = element.Rotate(value: 30f).Fade(value: 0.5).Blur(value: 5);

    anim.Completed += animation_completed;

    anim.Start();

{% endhighlight %}

And if you want to stop an animation before it ends, jsut call `Stop()`:

{% highlight csharp %}

    var anim = element.Rotate(value: 30f).Fade(value: 0.5).Blur(value: 5);
    anim.Start();

    anim.Stop();

{% endhighlight %}

## How does it work under the hood?

Animations can be done using XAML storyboards or Windows Composition.
By default the toolkit will use XAML storyboards unless you set *AnimationSet.UseComposition = true*.

### Using Windows Composition

While Windows Composition is faster and more efficient than XAML storyboards, it is important to understand several drawbacks that you may face when using it.


If you are using SDK 10586, Windows Composition and XAML storyboards behave exactly in the same way.


If you are using SDK 14393, the interoperabilty between XAML and Windows Composition changed (as stated by this [article](https://github.com/Microsoft/WindowsUIDevLabs/wiki/XAML-Composition-Interop-Behavior-Changes)).
In a nutshell, animating Offset and opacity with Windows Composition is only recommended if you do not change these states on XAML side. 
If you want to use Windows Composition and animate offset, then the safest way is to use a layout in XAML which positions the element at 0,0.
same for opacity where it is recommended to not define it in XAML.


### Offset, Scale and Rotate

When using storyboards for offset, scale and rotate, the toolkit will generate a CompositeTransform for you and will merge it with the current UIElement.RenderTransform (using a TransformGroup).
This means that you do not have to worry about the current state of your UIElement because the toolkit will take care of keeping it unchanged.

### Getting Started

Read the [getting Started with the UWP Community Toolkit]({{site.baseurl}}/{{page.lang}}/getting-started.htm) for instructions on using these API functions in your own projects. 

### Windows 10 Store App

Want to see the controls and animations in action before jumping into the code?  We have published the [UWP Community Toolkit Sample App](http://aka.ms/uwptoolkitapp) to the Windows 10 store.  Download the app and play with the controls live to see what they do before ever writing a line of code.

### GitHub Repository

Visit the [UWP Community Toolkit Github Repository](http://aka.ms/uwptoolkit) to see the current source code, what is coming next, and to clone the repository.  Community contributions are welcome!
