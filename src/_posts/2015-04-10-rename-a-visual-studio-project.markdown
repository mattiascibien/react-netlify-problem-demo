---
layout: post
title: Rename a Visual Studio Project
date: '2015-04-10 10:56:35'
tags: [programming, visual studio]
---

One of the problems beginners face when using Visual Studio happens when they try to rename a project since there will be a lot of leftovers in the process. This can be a problem even for professionals if they find out that the project name cannot be used, for example, in patents or copyright situations. Today we are going to fully rename a Visual Studio Project.

> Note: This guide works with every version of Visual Studio 
> and every kind of .NET Project.

## Step 1: Solution Name and Project Name
Renaming the solution is actually the simplest part of the process. Just click on the solution item in __Solution Explorer__ twice (but do not double click) to get an editable field and then type the new name.

In most of the cases your project name will match your solution name so just repeat the steps on the project item instead of the solution.

## Step 2: Folder Name
Renaming the project actually does not change the folder your poject is contained. When you do the first step you will have this situation:

```
<root>
|- NewName.sln
|- OldName
   |- NewName.csproj (or vbporj, vcxproj...)
```

In order to get the new name on the project folder you have to:

1. Rename the folder itself
2. Open the sln file with a text editor like NotePad and do a __Find&Replace__ to replace the old name with the new name.

> Note: You can also remove the wrong project inside __Soluton Explorer__ and add the correct one back.

## Step 3: Executable or Library Name
Executable (or Library) Name is actually preety easy to do: just right-click on your project in __Solution Explorer__ and choose __Properties__. 

In the application ta you will see the __Assembly Name:__ textbox. Just change these and you are ready to go

## Step 4: Namespaces
You may not want to keep the namespaces containing the name of your application, especially if you are using a name that you cannot use.

To do this, first of all, change the __Default Namespace__ in the project properties like you did in _Step 3_. and then you can use __File&Replace__ to change any reference to the old name in the new one. Alternatively you can rename the namespace in one of your files and then use the refractoring tool (the little box appearing under the namespace when you edit it) to replace any reference.

## Step 5: Enjoy
You have successfuly removed any reference to the old name in your project. Sit back, enjoy it and if you have any problem or question do not hesitate to contact me.

Mattias Out.