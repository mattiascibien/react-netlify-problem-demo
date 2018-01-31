---
layout: post
title: 'Upgrading from Visual C++ 6.0: The $(InputFile) macro'
date: '2015-09-30 18:10:00'
tags: [programming, visual studio]
---
When trying to compile code that used to run under Visual C++ 6.0 you actually
have to face some quirks which in particoular resides in custom build tools. 
One of these is the $(InputFile) macro producing linking errors like 
`cannot find input file '.\debug\.obj'`.

As the geek I tend to be, I like to do a lot of crazy things including compiling
old games with the modern compiler. 

Recently, when I was compiling the code of [Quake](https://github.com/id-Software/Quake)
under Visual C++ 2015, I faced the same problem I had with older versions of the IDE:
when the linker tries to link the output files of the Assembler, if fails with 
an error code similar to this:

```
Error: cannot find input file '.\debug\.obj'
```

The problem arises since the macro `$(InputFile)` is not available anymore in 
modern Visual C++ versions (therefore it produces an empty string as output). The
conversion process, moreover, does not manage to convert the macro occurences in the 
**Outputs** property of the Custom Build Tool.

Fixing this is as simple as opening the **Properties** of the files, and looking
into the **Outputs** of the custom build tool and replace the occurence of `$(InputFile)`
with the new `%(FileName)` macro which achieves the same effect. 
A screenshot of the final result can be seen in the image.

<img data-src="//res.cloudinary.com/mattiascibien/image/upload/v1443620784/visual_studio_cbt_gtqgws.png" class="img-responsive cld-responsive">

Hope that this trick will help you in bringing your old code into the new age.

Mattias Out.