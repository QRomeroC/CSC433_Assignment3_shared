Template code for A05
------------

Author: Arron Posey [@email.arizona.edu]
		Cesar D. Quihuis-Romero [qromeroc@arizona.edu]
Date: March, 2026

**PLEASE UPDATE THIS README**

You need to apply different shadings to the OBJ file.

***bugs and functionality**
Still tackling a bug regarding ambient color and diffusion. Diffusion shading is 
over saturating and not enough ambient is coming through, adjusting our color composition
to have more ambient and less diffusion. 

Included files (**PLEASE ADD/UPDATE THIS LIST**):
* materials/ -- a folder with different obj files, one texture, and one scene
* a03.js -- the main rendering codes
* m4.js -- the JS file which contains math functions for 4x4 matrices. The output matrices are by default Float32Array
* OBJFile.js -- the parser for OBJ files, another parser is provided in "a03.js". Use the one that you prefer
* webgl-utils.js -- the file containing utilities for making shader program and sending data to GPU
* png.js -- library to read PNG files
* GIFEncoder.js, LZWEncoder.js, and NeuQuant.js -- library to create GIF file


PLEASE PROVIDE ANY ATTRIBUTION HERE**
* First Obj parser: https://webglfundamentals.org/
* Second Obj parser: https://github.com/WesUnwin/obj-file-parser
* The library for decoding PNG files is from: https://github.com/arian/pngjs
* webgl-utils.js is from: GFXFundamentals
* The example obj files are from Blender and 3DsMax softwares
* GIFEncoder.js, LZWEncoder.js, and NeuQuant.js are from https://github.com/antimatter15/jsgif


**resources utlized to navigate implamentation of webGL**
uniformMatrix[2,3,4]fv(): (with example reference)
https://developer.mozilla.org/en-US/docs/Web/API/WebGLRenderingContext/uniformMatrix
https://developer.mozilla.org/en-US/docs/Web/API/WebGL2RenderingContext/uniformMatrix#examples

getUniform():
https://developer.mozilla.org/en-US/docs/Web/API/WebGLRenderingContext/getUniform

getUniformLocation():
https://developer.mozilla.org/en-US/docs/Web/API/WebGLRenderingContext/getUniformLocation

getProgramParameter():
https://developer.mozilla.org/en-US/docs/Web/API/WebGLRenderingContext/getProgramParameter

GL_ACTIVE_ATTRIBUTES:
https://registry.khronos.org/OpenGL-Refpages/gl4/html/glGetActiveAttrib.xhtml

getActiveAttrib():
https://developer.mozilla.org/en-US/docs/Web/API/WebGLRenderingContext/getActiveAttrib

exmple of where to set attributes/uniforms:
https://stackoverflow.com/questions/23967959/webgl-example-of-where-to-set-attributes-uniforms

how to get uniform values webgl:
https://stackoverflow.com/questions/58449060/how-to-get-uniform-value-from-webgl-shader-with-javascript-code

Discussion on what uniform and VAO are:
https://www.pouet.net/topic.php?which=8856&page=1

webGL tutorial:
https://developer.mozilla.org/en-US/docs/Web/API/WebGL_API/Tutorial

webGL: 2D and 3D basics:
https://developer.mozilla.org/en-US/docs/Web/API/WebGL_API

webGL(2) documenation (was using both gl1 and gl2 documenation):
https://registry.khronos.org/webgl/specs/latest/1.0/#5.14.10

webgl1 fundamentals:
https://webglfundamentals.org/webgl/lessons/webgl-3d-lighting-directional.html
https://webglfundamentals.org/webgl/lessons/webgl-attributes.html

webgl2 fundamentals (understand that gl2 was not used but still used to help):
https://webgl2fundamentals.org
https://webgl2fundamentals.org/webgl/lessons/webgl-fundamentals.html

webGL2 attributes:
https://webgl2fundamentals.org/webgl/lessons/webgl-attributes.html

webgl-3d-math:
https://webgl2fundamentals.org/docs/module-webgl-3d-math.html#.dot