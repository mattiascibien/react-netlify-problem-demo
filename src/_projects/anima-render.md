---
title: Anima Render
id: anima-render
tagline: OpenGL 2.0+ Renderer
ismin: false
details:
    website: http://mattiascibien.github.io/Anima-Render
    github: https://github.com/mattiascibien/Anima-Render
---

<img data-src="//res.cloudinary.com/mattiascibien/image/upload/w_auto/v1444231386/AnimaRender_2_ucwwsh.png" 
class="img-responsive cld-responsive" />

Anima Render is a OpenGL 2.0 scene renderer that started as a 
university project and then eveolved into an open-source (BSD licensed) one.

It has a proprietary file format similar to JSON to describe the scene and
has support for rendering obj models with custom shaders support and full screen
effects like Blur, Sharpen and much more.

Here is a sample scene file.

```
Camera {
	position 0.0 0.0 2.0
	direction 0.0 0.0 -1.0
	up 0.0 1.0 0.0
	FOVy 45
	screenEffect "screeneffects/sharpen3x3"
}

Transform {
	translation 0 0 0
	rotation 0 0 0 0
	scale 1 1 1 

	Object {
		geometry "geometries/cube_st.obj"
		material "martials/BlinnPhongDiffuse"
		params "ambient=0.1,0.1,0.1,1.0;shininess=51.2"
		texture0 diffuseTexture "textures/flowers.bmp"
	}
}
```

### Features

 * Rendering of obj models
 * Support for TGA, PNG and BMP textures
 * Experimental support for drawing optimized primitives
    * Cube
    * Quad
    * Geosphere
    * Tesselated sphere
 * Support for shaders including fullscreen effects
 * PhongBlinn Lighting
 * Cook Torrance Lighing
 * Multiple cameras (cycle with 'O' and 'P')


### Planned features

 * Normal mapping shader
 * Support for Linux and MacOS (technically the engine is cross-platform, but the
   project is based on the Visual Studio build system with NuGet for package
   management)

### Current Status

This project is actually on hold but contributions and suggestions are welcome.
They will implemented as soon as possibile. The successor has also been in the works
for some time, even if it is more a game engine rather than a renderer and the
licensing model is not decided yet.