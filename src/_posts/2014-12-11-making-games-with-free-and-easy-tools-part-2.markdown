---
layout: post
title: Making games easily with free tools (Part 2)
date: '2014-12-11 14:45:12'
tags:  [introduction, game making, clickteam fusion, zgameeditor]
---
Welcome back, my fellow readers. Today we are going to continue exploring the 
fantastic world of game making with other two fantastic programs: 
[ClickTeam Fusion](http://www.clickteam.com) and [ZGameEditor](http://www.zgameeditor.org/).

> Note: in case you missed it here is [part one]({% post_url 2014-10-26-making-games-with-free-and-easy-tools-part-1 %}).

## [Clickteam Fusion](http://www.clickteam.com)

<div class="embed-responsive embed-responsive-16by9" style="max-width: 85%;">
    <iframe class="embed-responsive-item" src="//www.youtube.com/embed/XYQL1jL50qI" frameborder="0" allowfullscreen></iframe>
</div>

Clickteam Fusion is the latest installment of a series of game developing tools made by Clickteam and the successor of Multimedia Fusion 2.

Like the other tools I showed in the first part this one relies on the same concepts: design your levels with visual tools and then make the actors interact with the environment and between themselves. Can you guess how? By defining a list of actions for any event.

The level (frame) editor is quite similar to the the brothers' ones so I am not going to delve deeper into it: just drag the objects from the bottom panel or create new one by righ-clicking.

Events and actions instead, are defined in a user interface split in two different parts: the __Event Editor__, a table-like environment where an event is a row and, for every object (the colums of the table), actions are defined in the cells and the __Event List Editor__ which is actually a detailed view of a cell.

Clickteam fusion comes in three editions.

The free edition which can export to HTML5 and it's limited, a standard edition and the developer one which adds [some features](http://www.clickteam.com/compare-versions) to the standard and lifts you from the need to quote Clickteam in the features.

#### Pros

 - A lot of graphics and predefined objects included
 - Cheaper than other solutions
 - Easy (and funny) to use physics engine

#### Cons

 - Free edition has [some limitations](http://community.clickteam.com/threads/88310-Free-HTML5-edition-differences?p=639416&viewfull=1#post639416) and one in particoular can be pretty annoying (3 screen limit)
 - No native games in the free edition (you can still wrap an HTML5 game with [node-webkit](https://github.com/rogerwang/node-webkit) easily)
 - Event editor can be confusing
 - Expensive modules
 - Less available platforms than other solutions
 
#### Considerations
Although the program is still a valid and cheap option the free edition seems just a demo version, so if you do not want to deal with the limitations I suggest to try out [Game Maker: Studio](http://www.yoyogames.com) or [Construct 2](http://www.scirra.com).

I just actually scratched the surface of this program and I have not yet created a complete game with it, mostly because I keep using the previous version which is preety the same.

You should check out this piece of software and see if it fits you because it has a large user base and a lot of games (even paid ones like the [Five Nights at Freddy's series](http://clickstore.clickteam.com/games/five-nights-at-freddys)) have been made with it.

## [ZGameEditor](http://www.zgameeditor.org/)

![](http://zgameeditor.org/images/zge_shot2.png)

With ZGameEditor we drift away from the event-action approach and instead we delve deeper on how a game engine is built.

In simple words a game is actually just a big loop which works like this until the user quits it:

 - Read the user input (keyboard, joypad, mouse...)
 - Update the game world (AI actions, increase score...)
 - Draw everything on the screen
 
All the programs I have showed until now actually work on a higher level and you mostly do not happen to work at the lower levels.

What you actually see on the tree on the left of the screen is nothing more than a series of actions (the ones beginning with _On_) which will get executed in a loop, accompanied by some Content.

This almost "bare metal" approach can be scary if you are just beginning in game developmet and is trickier than the event-action approach but, if you open up any of the included samples and read a getting started guide, you will master the basic functions without problems. Moreover you will learn both the basics of an advanced game engine and of 3D graphics.

ZGameEditor lets you even export your games on PC (Windows, Mac and Linux) and mobile (Android) for free.

#### Pros
 - Open Source software
 - Easier 3D than competitors
 - Teaches game engine concepts
 - Produces very light games (just one little executable)
 
#### Cons
 - Non-frequent releases
 - Steeper learning curve
 
 
Hoping that you will find this new guide useful, see you with the next part.