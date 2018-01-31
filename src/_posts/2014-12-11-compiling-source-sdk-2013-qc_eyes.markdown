---
layout: post
title: Compiling Source SDK 2013 QC_Eyes
date: '2014-12-11 10:13:33'
tags: [programming, visual studio, half-life 2, source sdk, mfc]
---

Today I wished to see if I could still be able to compile the [Source SDK](https://github.com/ValveSoftware/source-sdk-2013) and I made it. It just had a little problem with QC_Eyes using Visual Studio 2013.

First when you try to compile it you will receive an error about missing `nafxcwd.lib`, which is related to [Microsoft Foundation Classes](http://it.wikipedia.org/wiki/Microsoft_Foundation_Classes). In particoular QC_Eyes is supposed to be compiled using the **Mult-Byte Character Set** version of MFC, which is deprecated in the latest version of Visual Studio.

The fix for this is actually pretty simple as said in an official Microsoft post ([reference](http://blogs.msdn.com/b/vcblog/archive/2013/07/08/mfc-support-for-mbcs-deprecated-in-visual-studio-2013.aspx?PageIndex=3)).

Just install the package linked [here](http://go.microsoft.com/?linkid=9832071) and you are ready to go.

Hope to have helped you.
Mattias