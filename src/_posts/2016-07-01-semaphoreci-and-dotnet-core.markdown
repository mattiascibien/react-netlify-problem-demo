---
layout: post
title: 'SemaphoreCI and .NET Core'
date: '2016-07-01 00:00:00'
tags: [programming, dotnetcore, dotnet]
---

In this post we are going to examine how [SemaphoreCI](https://semaphoreci.com/) can help us build and test 
[.NET Core](https://www.microsoft.com/net/core) projects.

With the release of .NET Core 1.0, Microsoft opened the world of .NET Managed Programming to 
other Operating Systems including Linux, which is the ones most of Clouds like [Openshift](https://www.openshift.com/) 
or [DigitalOcean](https://m.do.co/c/a2eb7e4a08d0) rely on.

This also means that you can use the most famous continous integration services to automatically
build, test and even deploy .NET Core applications.

In this tutorial I am going to focus on [SemaphoreCI](https://semaphoreci.com/) as it is the one I am using right now
and also provides 100 free builds/month even for private projects. 
For more information you can check their [pricing page](https://semaphoreci.com/pricing).

Building your .NET projects is really simple. Just add you Github or Bitucket project to Semaphore
and use the following steps to the build language.

First you must set the Language to **Other** and then you should add the following lines to 
the Setup Thread:

```
sudo sh -c 'echo "deb [arch=amd64] https://apt-mo.trafficmanager.net/repos/dotnet/ trusty main" > /etc/apt/sources.list.d/dotnetdev.list'
sudo apt-key adv --keyserver apt-mo.trafficmanager.net --recv-keys 417A0893
sudo apt-get update
sudo apt-get install -y dotnet-dev-1.0.0-preview2-003121
```
These are the same lines form the [.NET Core install](https://www.microsoft.com/net/core#ubuntu) 
page that does not require user input. After doing this you can customize your *Thread#1* to do the
standard .NET build and test commands:

```
cd ./src/[YourProjectName]
dotnet build
cd ../../test/[YourProjectName].Tests
dotnet test
cd ..../src/[YourProjectName]
dotnet publish
```

Your project will now be compiled, published and unit tested. If you face any problems just drop a comment
here and I will be glad to help you.