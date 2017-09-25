.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

set()
=====

Set the color of a single pixel or write an image into
this p5.Image.
Note that for a large number of pixels this will
be slower than directly manipulating the pixels array
and then calling updatePixels().

**รูปแบบการใช้งาน**

set ( x, y, a )

**พารามิเตอร์**

- ``x``  Number: x-coordinate of the pixel

- ``y``  Number: y-coordinate of the pixel

- ``a``  Number,Array,Object: grayscale value | pixel array | a p5.Color | image to copy


.. raw:: html

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

.. toctree::

