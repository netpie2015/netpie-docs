.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

blend()
=======

Copies a region of pixels from one image to another, using a specified
blend mode to do the operation.

Available blend modes are: BLEND | DARKEST | LIGHTEST | DIFFERENCE |
MULTIPLY| EXCLUSION | SCREEN | REPLACE | OVERLAY | HARD_LIGHT |
SOFT_LIGHT | DODGE | BURN | ADD | NORMAL

**รูปแบบการใช้งาน**

blend ( srcImage, sx, sy, sw, sh, dx, dy, dw, dh, blendMode )

**พารามิเตอร์**

- ``srcImage``  : source image

- ``sx``  : X coordinate of the source's upper left corner

- ``sy``  : Y coordinate of the source's upper left corner

- ``sw``  : source image width

- ``sh``  : source image height

- ``dx``  : X coordinate of the destination's upper left corner

- ``dy``  : Y coordinate of the destination's upper left corner

- ``dw``  : destination image width

- ``dh``  : destination image height

- ``blendMode``  : the blend mode


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var img0;
	var img1;
	
	function preload() {
	  img0 = loadImage("assets/rockies.jpg");
	  img1 = loadImage("assets/bricks_third.jpg");
	}
	
	function setup() {
	  background(img0);
	  image(img1, 0, 0);
	  blend(img1, 0, 0, 33, 100, 67, 0, 33, 100, LIGHTEST);
	}
	var img0;
	var img1;
	
	function preload() {
	  img0 = loadImage("assets/rockies.jpg");
	  img1 = loadImage("assets/bricks_third.jpg");
	}
	
	function setup() {
	  background(img0);
	  image(img1, 0, 0);
	  blend(img1, 0, 0, 33, 100, 67, 0, 33, 100, DARKEST);
	}
	var img0;
	var img1;
	
	function preload() {
	  img0 = loadImage("assets/rockies.jpg");
	  img1 = loadImage("assets/bricks_third.jpg");
	}
	
	function setup() {
	  background(img0);
	  image(img1, 0, 0);
	  blend(img1, 0, 0, 33, 100, 67, 0, 33, 100, ADD);
	}
	</script>

	<br><br>

.. toctree::

