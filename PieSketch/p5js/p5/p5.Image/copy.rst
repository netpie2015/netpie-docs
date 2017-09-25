.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

copy()
======

Copies a region of pixels from one image to another. If no
srcImage is specified this is used as the source. If the source
and destination regions aren't the same size, it will
automatically resize source pixels to fit the specified
target region.

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


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var photo;
	var bricks;
	var x;
	var y;
	
	function preload() {
	  photo = loadImage("assets/rockies.jpg");
	  bricks = loadImage("assets/bricks.jpg");
	}
	
	function setup() {
	  x = bricks.width/2;
	  y = bricks.height/2;
	  photo.copy(bricks, 0, 0, x, y, 0, 0, x, y);
	  image(photo, 0, 0);
	}

	</script>

	<br><br>

.. toctree::

