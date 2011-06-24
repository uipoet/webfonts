Web Fonts
=========

Create fonts for web browsers.

Installation
------------

	npm install webfonts

Usage
-----

	webfonts -h

About
-----

Web fonts takes a directory containing ttf(TrueType Font) files and generates woff, eot and svg font files for cross-browser web font embedding via CSS.

You may either change to the fonts directory and simply run the command `webfonts` or run the command from anywhere followed by the path to the fonts directory.

By default the web fonts will be generated into the original fonts directory. You may optionally add the -o followed by a path to copy the original ttfs and generate the web fonts into a different directory.

Recommended CSS for Embedding
-----------------------------

	@font-face {
	  font-family: '<Font Name>';
	  src: url('fonts/<fontname>.eot');
	  src: url('fonts/<fontname>.eot?iefix') format('eot'),
	    url('fonts/<fontname>.woff') format('woff'),
	    url('fonts/<fontname>.ttf') format('truetype'),
	    url('fonts/<fontname>.svg#<fontname>') format('svg');
	  font-style: normal;
	  font-weight: normal;
	}

Dependencies
------------

[Node.js](http://nodejs.org/)

[Java](http://www.java.com/)

Included Libraries
------------------
[sfnt2woff](http://people.mozilla.org/~jkew/woff/)

[ttf2eot](http://code.google.com/p/ttf2eot/)

[batik-ttf2svg](http://xmlgraphics.apache.org/batik/tools/font-converter.html)


License
-------

Copyright 2011 Jamie Hoover

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.

You may obtain a copy of the License at

[apache.org/licenses/LICENSE-2.0](http://www.apache.org/licenses/LICENSE-2.0)

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.
