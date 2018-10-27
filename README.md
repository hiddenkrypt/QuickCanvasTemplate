# quickcanvas template

A "starting point" that I find common to many little quick canvas programs I've been making. This is more or less my boilerplate for getting canvas games started, even if it's not great for final products.

The html file has a canvas element with a border, centered. It also has four div tags for outputting whatever is needed. It pulls in the drabble.js and code.js files.

drabble.js sets up a window.onload function to grab references to the divs and canvas, and create a canvas 2d context. It also calls a function named "init", which is defined in code.js. As helper utilities, drabble includes an object for common keycode names that used to be more useful, and a shim for requestAnimationFrame which used to be more necessary.

code.js is almost entirely empty, only having a function named init() with no body. This is where game code begins. init() is called by the window.onload function set up in drabble.js. 
