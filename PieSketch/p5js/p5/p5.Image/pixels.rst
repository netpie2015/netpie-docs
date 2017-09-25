.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

pixels
========

Array containing the values for all the pixels in the display window.
These values are numbers. This array is the size (include an appropriate
factor for pixelDensity) of the display window x4,
representing the R, G, B, A values in order for each pixel, moving from
left to right across each row, then down each column. Retina and other
high denisty displays may have more pixels[] (by a factor of
pixelDensity^2).
For example, if the image is 100x100 pixels, there will be 40,000. With
pixelDensity = 2, there will be 160,000. The first four values
(indices 0-3) in the array will be the R, G, B, A values of the pixel at
(0, 0). The second four values (indices 4-7) will contain the R, G, B, A
values of the pixel at (1, 0). More generally, to set values for a pixel
at (x, y):
```javascript
var d = pixelDensity;
for (var i = 0; i < d; i++) {
  for (var j = 0; j < d; j++) {
    // loop over
    idx = 4 * ((y * d + j) * width * d + (x * d + i));
    pixels[idx] = r;
    pixels[idx+1] = g;
    pixels[idx+2] = b;
    pixels[idx+3] = a;
  }
}
```

Before accessing this array, the data must loaded with the loadPixels()
function. After the array data has been modified, the updatePixels()
function must be run to update the changes.

**รูปแบบการใช้งาน**

pixels

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	img = createImage(66, 66);
	img.loadPixels();
	for (i = 0; i < img.width; i++) {
	  for (j = 0; j < img.height; j++) {
	    img.set(i, j, color(0, 90, 102));
	  }
	}
	img.updatePixels();
	image(img, 17, 17);

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var pink = color(255, 102, 204);
	img = createImage(66, 66);
	img.loadPixels();
	for (var i = 0; i < 4*(width*height/2); i+=4) {
	  img.pixels[i] = red(pink);
	  img.pixels[i+1] = green(pink);
	  img.pixels[i+2] = blue(pink);
	  img.pixels[i+3] = alpha(pink);
	}
	img.updatePixels();
	image(img, 17, 17);

	</script>

	<br><br>

.. toctree::

