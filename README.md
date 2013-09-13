# bloody-grid v0.1 #

Bloody grid is a full-screen mosaic responsive web grid layout inspired by [Raymond Weil Inspiration](http://inspiration.raymond-weil.com/#!/inspiration "Raymond Weil") web page.

## Examples ##

* (Not yet)

## Features ##

* (Almost!) fully configurable settings.
* CSS-only library.
* Use only markup attributes to control grid blocks. (No additional CSS positioning required.)
* Tested in IE 8+, Chrome, Safari, Firefox

## Requirements ##

* [Stylus](https://github.com/learnboost/stylus "Stylus") (Tested on 0.36.1)

## Setup ##

1. Adjust `settings.styl` to set available grid mode to meet your needs. You can edit : 
   1. Number of columns and corresponding options each (maximum available rows, min-max width)
   2. Default number of columns. (Fallback for ie8)
   3. Width-height ratio of a single cell.
   4. Largest width, height of a single cell.
   5. Classname and prefix that bloody-grid will use.
2. Compile stylus file. 
3. In your markup, add the `.bloody-grid` container :
   1. Set the width and height of each gridset on the grid container. 
      e.g. `data-bg-rows-3="10" data-bg-rows-5="7" data-bg-rows-7="4"`
   2. Set the width and height of each cell on the grid container. 
      e.g. `data-bg-size="2x2"`
   3. Set the position of each cell on the grid container for each gridset. Use hide to hide an element. 
      e.g. `data-bg-3="hide" data-bg-5="2,0" data-bg-7="0,3"`
4. Test!

## Known Bugs ##

* Safari has a ~1px error on positioning grid elements causing space between each cells.