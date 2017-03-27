## Why Use SVGs?

* Vector = retina without _2x files
* Lightweight = file tells browser how to draw shapes, not long, unreadable lists of raw pixel data
* CSS style modifications
* Better than icon fonts = user font-disabling, quality, load time

## Generating SVGs

### Copy-Paste from Illustrator
* Select group & copy
* Open Sublime Text new file & paste
* Profit!!

### Export from Illustrator
### Other Issues
* Icon font characters? Type -> Create Outlines
* Multiple Icons? Save as individual files: not sprite sheets
* Colors? Shapes should be filled and/or stroked with most frequently used color: we can change color for edge cases with CSS

## Optimizing SVGs
 
Nobody does a thing! (Our front-end Gulp script does it all for us!)

## Using SVGs in WordPress
 
Upload to Media Library (not optimized by the script - need a plugin for that)

Use in theme `/img/` directory (optimized by script, but * inaccessible to Design/Marketing/Content)

* `get_svg()` function makes SVG markup available to inline in page * content
* Elements inside inline SVGs can be styled with CSS properties and * respond to media queries & hover interactions