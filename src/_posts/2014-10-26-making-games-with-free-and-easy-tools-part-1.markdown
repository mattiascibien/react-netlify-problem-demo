---
layout: post
title: Making games easily with free tools (Part 1)
date: '2014-10-26 08:09:34'
tags: [introduction, game making, game maker, construct]
---

This article has been in the works for quite some time now and finally I decided to make it into a series. In every part of the series I am going to introduce you, my fellow readers, to some of the tools for creating games, both for beginner and advanced users.

Have you ever wondered how the games you play on your PC are made and wondered to create your own? If you know the right tools, this could be a very easy task and, if you are brave enough, you can even earn some extra money.

Let's now introduce some nice game making tools that you can use to express your creativity and challenge your brain without having to work with complex environments.

## [Game Maker: Studio](http://www.yoyogames.com)
![Game Maker Studio](//res.cloudinary.com/mattiascibien/image/upload/v1439915542/game-maker_pc_2153_dx92sr.png)

I am going to start with [Game Maker: Studio](https://www.yoyogames.com/) since I have a very special relationship with it: it was in fact the first program I used to create my first game.

I was actually 12 years old when I coded my first one-brick breakout clone and it took only one hour to make it. Ok, it was not a complete game but this was the proof that Game Maker learning curve is not steep.

The concepts behind it are simple: drag your actors (objects) with an associated look (sprite) into a level (room) and make them react to the envirnoment events (using actions). Here is an example screenshot of a simple object:

![Game Maker Studio: Events and Actions](//res.cloudinary.com/mattiascibien/image/upload/v1439915470/object_pavl9y.png)

Everything is done via drag-and-dop actions. If you want do delve deeper you can even use the included complete code editor for the program programming language (GML).

When you are done with your game you can export it by using the _Create Executable_ menu entry to be played on your PC (Windows, MAC, Linux), on the Web, on your Phone (Android, Windows Phone, iOS, Tizen) or on your tablet (Windows 8, Windows RT, Android, iOS) and distribute it to your friends or upload it to the app stores.

Unfortunately most of the platform you are not available for free. Game Maker: Studio, in fact, comes in different editions to suite your needs.

The first (and completely free) is the __Standard Edition__ which is feature limited (you will not need the missing features anyway if you are just scratching the surface) and can export only for Windows (Desktop only, not Tablet).

> Note: Standard Edition was once _$49_ and included Windows Tablets and Mac export, but when it became free those features where removed.

The __Professional Edition__ (_$99_) comes with all the features of the Standard one plus some additions needed mostly for advanced users (like texture and configuration management) and lets you export for Windows Tablets.

Additional exporters are available as separate products and [prices](https://www.yoyogames.com/studio) go from _99$_ to _299$_.

In addition to this you can get the __Master Collection__ (_$799_) containing the all of the exporters (including future ones).

A detailed feature comparison for all edition can be found on the [official page](https://www.yoyogames.com/studio).

Moreover the authors has announced some fantastic new features coming in the next months including:
 
 - [Compilers](http://www.yoyogames.com/news/240) for some exporters (read: performance improvements)
 - [Game Maker: Player](https://yoyogames.com/news/239) (online game share platform)
 - [Support for the latest Windows platforms](http://www.yoyogames.com/company/press/releases/33) (8.1, Phone 8.1 and hopefully 10)

#### Pros
 - Very easy to learn
 - Integrated tutorials
 - Visual editors for everything
 - Code editor for advanced users
 - Extensible
 - Integrations with third party services like ad providers and [Steamworks](http://www.steampowered.com/steamworks/)
 - Comes with an included [Asset Marketplace](https://marketplace.yoyogames.com/)

#### Cons
 - Damn expensive for non-Windows platforms (with compilers prices are being increased)
 - Still lack of support for Windows 8.1 Apps (they say it is on its way, though)
 
## [Construct 2](http://www.scirra.com)
![Construct 2](//res.cloudinary.com/mattiascibien/image/upload/v1439915353/construct2_vc0u3f.png)

I discovered Construct 2 during my last year at university when the company behind it held a [competition](https://www.scirra.com/blog/104/new-windows-8-game-competition) on Windows 8, so I made [Boh! Jungle Fever](http://apps.microsoft.com/windows/en-us/app/boh-junlge-fever/59e397cb-1988-4714-9b9e-43a8db9a046b).

The program is preety similar to Game Maker in many ways, featuring visual editors for graphics and for levels.

The way you make objects interact with each other, though, is fairly different. You still have to define how an object responds to external events but for common game concepts like jumping, moving on platforms, car movement and more you have some predefined behaviours: just drop one into your object and they will "magically" work like that.

![Construct 2: Behaviours](//res.cloudinary.com/mattiascibien/image/upload/v1439915357/behaviours_wqgo5u.png)

Once you have defined how your objects behave you just need to define how they interact with each other using the event sheet. When you are done just hit _Export Project_ and publish your game; there are [many platforms](https://www.scirra.com/construct2#multi) to choose.

This program is available in three editions: 
 
 - A __Free__ one with [limited functionality](https://www.scirra.com/store/construct-2/page-1) and limited to free games
 - A __Personal__ one available for _$129,99_, suitable for indipendent developers with revenue less than $5.000 USD.
 - A __Business__ one available for _$429,99_, for companies and individuals that cannot suit Personal License terms

#### Pros
 - Available for many platforms
 - Cheaper than other solutions (all exporters are available in the paid editons) 
 - Predefined behaviours help getting a working game in no time
 
#### Cons
 - Free edition has some limits but in most cases they will not make the developer suffer
 - Exporters for Desktop, Android (except Amazon Store), Blackberry and iOS are not free
 - Monetizing your game is prohibited by using the free version
 - Exported games are HTML5 (web) apps wrapped in native containers (read: less performance than pure native apps, like Game Maker ones)
 - Event editor is more caothic than Game Maker's one
 
This are just two of the many game development tools you can find and many of them will be examined with the following parts.

See you with [Part 2]({% post_url 2014-12-11-making-games-with-free-and-easy-tools-part-2 %}).

Mattias.
 