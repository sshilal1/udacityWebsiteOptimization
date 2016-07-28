## Website Performance Optimization portfolio project

## To Run Project: Click on index.html

### Part 1: Optimize PageSpeed Insights score for index.html

1. Removed Google Webfonts, saved multiple seconds
2. Minified CSS
3. Made both JS scripts load asynchronously
4. Compressed images using compressor.io

### Part 2: Optimize Frames per Second in pizza.html

1. Optimized For Loop
	* Max was 30 fps, now max is 40 fps while scrolling
2. Debouncing Scroll events. 'debounce' section of http://www.html5rocks.com/en/tutorials/speed/scrolling/
	* Stored last value of scroll position
	* Performed updates inside a requestanimationframe using last value of scroll position
	* Succesfully scroll at 60 fps
3. Resizing pizzas is at an average of .7ms, which is less than the required 5ms
4. Adjusted pizza background renderings based on the window height, instead of 200 always.
	* THis brought it from 59.9 to a stable 60 fps