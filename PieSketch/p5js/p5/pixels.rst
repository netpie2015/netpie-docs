.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

pixels
========

Uint8ClampedArray
containing the values for all the pixels in the display window.
These values are numbers. This array is the size (include an appropriate
factor for pixelDensity) of the display window x4,
representing the R, G, B, A values in order for each pixel, moving from
left to right across each row, then down each column. Retina and other
high density displays will have more pixels[] (by a factor of
pixelDensity^2).
For example, if the image is 100x100 pixels, there will be 40,000. On a
retina display, there will be 160,000.

The first four values (indices 0-3) in the array will be the R, G, B, A
values of the pixel at (0, 0). The second four values (indices 4-7) will
contain the R, G, B, A values of the pixel at (1, 0). More generally, to
set values for a pixel at (x, y):
```javascript
var d = pixelDensity();
for (var i = 0; i While the above method is complex, it is flexible enough to work with
any pixelDensity. Note that set() will automatically take care of
setting all the appropriate values in pixels[] for a given (x, y) at
any pixelDensity, but the performance may not be as fast when lots of
modifications are made to the pixel array.

Before accessing this array, the data must loaded with the loadPixels()
function. After the array data has been modified, the updatePixels()
function must be run to update the changes.

Note that this is not a standard javascript array.  This means that
standard javascript functions such as slice() or
arrayCopy() do not
work.

**รูปแบบการใช้งาน**

pixels

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var pink = color(255, 102, 204);
	loadPixels();
	var d = pixelDensity();
	var halfImage = 4 * (width * d) * (height/2 * d);
	for (var i = 0; i < halfImage; i+=4) {
	  pixels[i] = red(pink);
	  pixels[i+1] = green(pink);
	  pixels[i+2] = blue(pink);
	  pixels[i+3] = alpha(pink);
	}
	updatePixels();

	</script>

	<br><br>

.. toctree::

