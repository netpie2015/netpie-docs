.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

createImage()
=============

Creates a new p5.Image (the datatype for storing images). This provides a
fresh buffer of pixels to play with. Set the size of the buffer with the
width and height parameters.

.pixels gives access to an array containing the values for all the pixels
in the display window.
These values are numbers. This array is the size (including an appropriate
factor for the pixelDensity) of the display window x4,
representing the R, G, B, A values in order for each pixel, moving from
left to right across each row, then down each column. See .pixels for
more info. It may also be simpler to use set() or get().

Before accessing the pixels of an image, the data must loaded with the
loadPixels() function. After the array data has been modified, the
updatePixels() function must be run to update the changes.

**รูปแบบการใช้งาน**

createImage ( width, height )

**พารามิเตอร์**

- ``width``  : width in pixels

- ``height``  : height in pixels


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
	
	img = createImage(66, 66);
	img.loadPixels();
	for (i = 0; i < img.width; i++) {
	  for (j = 0; j < img.height; j++) {
	    img.set(i, j, color(0, 90, 102, i % img.width * 2));
	  }
	}
	img.updatePixels();
	image(img, 17, 17);
	image(img, 34, 34);
	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	var pink = color(255, 102, 204);
	img = createImage(66, 66);
	img.loadPixels();
	var d = pixelDensity();
	var halfImage = 4 * (width * d) * (height/2 * d);
	for (var i = 0; i < halfImage; i+=4) {
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

