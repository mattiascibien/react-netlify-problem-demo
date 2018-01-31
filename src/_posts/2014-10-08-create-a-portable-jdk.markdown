---
layout: post
title: Create a Portable JDK for Eclipse
date: '2014-10-08 13:54:16'
tags: [tutorial, portable, java, jdk]
---

On my old blog I used to have an article on how to create a portable JDK in order to prevent to have it installed. I am reproducing it here as a reference for future readers.

I always hated Java since when I started using it in my browser: annoying updates, useless processes that slow down the system and 30MB of memory occupied by an application that does nothing are too much. I actually prefer .NET over Java, mostly for its perfomance, but sometimes you have to get your hands dirty in something you do not like so here I am with my Portable JDK (and even JRE if needed).

Even if Oracle does not tell you this the JDK is fully portable and can be moved anywhere you want without breaking the system so actually if you need it just to run Eclipse you can follow this steps to use it only in that case and you can remove it from your system (which is very nice if you are a Java hater like me):

- Install the JDK in the classic way.
- Get to the directory where you installed it (such as `C:\Program Files\Java\`) and copy the subdirectory `jdk1.7.0_10` in the eclipse folder.
- Edit `eclipse.ini` by adding those two lines at the very top of the file (be careful: they must be two lines)

        -vm
        .\jdk1.7.0_10\bin\javaw

- Run Eclipse and you will have a fully working development environment.
- Uninstall JDK


Have fun with your Eclipse and be sure to check out the source of this article (http://tgducusin.blogspot.it/2011/12/portable-eclipse-with-java-jdk-tomcat.html).

Mattias