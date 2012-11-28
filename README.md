webgl.d.ts
==========

A WebGL definition file for TypeScript. Generated with help of my own IDL exporttool [idl2typings](https://github.com/RicoP/idl2typings).

Example App


	///<reference path="webgl.d.ts" />

	window.onload = () => { 
		var canvas = <HTMLCanvasElement> document.createElement("canvas"); 
		document.body.appendChild(canvas); 

		var gl = canvas.getContext("experimental-webgl", {}); 

		gl.clearColor(1,0,0,1);
		gl.clear(gl.COLOR_BUFFER_BIT); 
	}


It's important to notice that the second parameter of getContext is mandatory so TypeScript can figure out that you want a WebGLContext and not a Canvas2DContext. 

This is a free library under the MIT license. I would love to hear from you when you use this lib :) 

LICENSE
=======
Copyright (C) 2012 Rico Possienka 

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.


[![Flattr this git repo](http://api.flattr.com/button/flattr-badge-large.png)](https://flattr.com/submit/auto?user_id=RicoTweet&url=https://github.com/RicoP/webgl.d.ts&title=webgl.d.ts&language=&tags=github&category=software)