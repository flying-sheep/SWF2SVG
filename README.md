SWF2SVG
=======
I observed with disbelief that there is no real, working way to extract the shapes in static SWF frames that doesn’t require heavy interaction.

There was a bunch of outdated or bad tools, e.g. [Steve Probets’](http://www.eprg.org/~sgp/swf2svg.html), [ALI G’s](http://swf2svg.sourceforge.net/) or some python script based on [SWFDUMP](http://www.swftools.org/).

There were complicated solutions that required much user interaction per conversion, such as printing the SWF to a PDF and using Inkscape to import that. I found one of these in this [Stackoverflow question](http://stackoverflow.com/questions/6542614/how-to-convert-a-swf-displayobject-to-svg-data), but it used [a library](https://github.com/claus/as3swf). And having recently heared about Adobe’s AIR, I made the connection.

And two days fiddling with a (for me) completely new technology, I present: SWF2SVG.

Usage
-----

	SWF2SVG file1.swf file2.swf …

creates

	file1.svg file2.svg …