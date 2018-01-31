---
title: Autocam for DAZ Studio
id: autocam
tagline: Automatic DAZ Cameras
ismin: false
---

AutoCam is a plug-in for DAZ Studio aimed at automatic camera placement in a 3D scene.

### The Original Project
AutoCam began a beachelor thesis project, developed at University of Udine 
under the mentoring of [Roberto Ranon](https://users.dimi.uniud.it/~roberto.ranon/). 
A copy of the paper is going to be available soon, written in italian.

The goal of this thesis was to develop a plug-in for DAZ Studio that was able to
place a camera (or viewpoint) in a 3D by using photographics properties like 
shot angle and shot lenght.

For example you can express properties like: 
a medium-length shot for that Genesis 2 charachter with a full-body shot for that Genesis one. 

The program itself is capable to find a camera that satisfies those properties.

### The new age

AutoCam is actually a complete rewrite of the original project with some additions
including, but not limited to:

 * Usage of the open source [SmartViewPointComputationLib](https://bitbucket.org/rranon/smart-viewpoint-computation-lib)
 * Better user interface
 * Customization of the original presets and tweaking of its properties
 * Possibility to create custom presets
 * Loading and saving of the state of the various aspects of the project in the DAZ Studio scene file

### Current Status

Unfortunately, due to lack of time, the project is currently on hold.

The original thesis source code cannot be released to the public due to licensing 
issues with the old version of SmartViewPointComputationLib (which is private).