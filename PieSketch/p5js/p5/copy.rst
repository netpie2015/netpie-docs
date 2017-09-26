.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

copy()
======

Copies a region of the canvas to another region of the canvas
and copies a region of pixels from an image used as the srcImg parameter
into the canvas srcImage is specified this is used as the source. If
the source and destination regions aren't the same size, it will
automatically resize source pixels to fit the specified
target region.

.. Copies a region of the canvas to another region of the canvas
.. and copies a region of pixels from an image used as the srcImg parameter
.. into the canvas srcImage is specified this is used as the source. If
.. the source and destination regions aren't the same size, it will
.. automatically resize source pixels to fit the specified
.. target region.
**รูปแบบการใช้งาน**

copy ( srcImage, sx, sy, sw, sh, dx, dy, dw, dh )

**พารามิเตอร์**

- ``srcImage``  p5.Image,undefined: source image

- ``sx``  Integer: X coordinate of the source's upper left corner

- ``sy``  Integer: Y coordinate of the source's upper left corner

- ``sw``  Integer: source image width

- ``sh``  Integer: source image height

- ``dx``  Integer: X coordinate of the destination's upper left corner

- ``dy``  Integer: Y coordinate of the destination's upper left corner

- ``dw``  Integer: destination image width

- ``dh``  Integer: destination image height

.. ``srcImage``  p5.Image,undefined: source image
.. ``sx``  Integer: X coordinate of the source's upper left corner
.. ``sy``  Integer: Y coordinate of the source's upper left corner
.. ``sw``  Integer: source image width
.. ``sh``  Integer: source image height
.. ``dx``  Integer: X coordinate of the destination's upper left corner
.. ``dy``  Integer: Y coordinate of the destination's upper left corner
.. ``dw``  Integer: destination image width
.. ``dh``  Integer: destination image height

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var img;
	
	function preload() {
	  img = loadImage("assets/rockies.jpg");
	}
	
	function setup() {
	  background(img);
	  copy(img, 7, 22, 10, 10, 35, 25, 50, 50);
	  stroke(255);
	  noFill();
	  // Rectangle shows area being copied
	  rect(7, 22, 10, 10);
	}

	</script>

	<br><br>

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
