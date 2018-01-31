---
layout: post
title: Cross-Platfom games with MonoGame, getting started
---

With the new features of Visual Studio 2013 and 2015 creating cross-platform games with [MonoGame](http://www.monogame.net/) became very easy. In this tutorial I am going to show how to use the new __Shared Project__ feature of the latest versions of the Microsoft IDE.

> Note: the screenshot here are made using Visual Studio 2015.
> The older version uses a different format for shared project and in some cases the process it is different. The differences will be highlighed during the tutorial. Also, [NuGet](http://nuget.org), will be used to handle MonoGame instead.

## Installing the Shared Project Extension
This step applies only on 2013 where Shared Projects can be used only in Windows Store Apps. With this extension, however, they can be used in any kind of project.

[Shared Project Reference Manager Extension](https://visualstudiogallery.msdn.microsoft.com/315c13a7-2787-4f57-bdf7-adae6ed54450)

## Install MonoGame
At the time of writing the latest version of MonoGame is __3.2__ which does not feature the Content Pipeline like XNA did. Since we do not want to install XNA Game Studio we are going to use the new Content Pipeline tool available in the latest [development build](http://www.monogame.net/downloads/).

> Note: When the new version comes out just get the latest stable.

## Create the first project


