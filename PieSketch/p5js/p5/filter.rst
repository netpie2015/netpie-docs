.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

filter()
========

Applies a filter to the canvas.


The presets options are:


THRESHOLD
Converts the image to black and white pixels depending if they are above or
below the threshold defined by the level parameter. The parameter must be
between 0.0 (black) and 1.0 (white). If no level is specified, 0.5 is used.


GRAY
Converts any colors in the image to grayscale equivalents. No parameter
is used.


OPAQUE
Sets the alpha channel to entirely opaque. No parameter is used.


INVERT
Sets each pixel to its inverse value. No parameter is used.


POSTERIZE
Limits each channel of the image to the number of colors specified as the
parameter. The parameter can be set to values between 2 and 255, but
results are most noticeable in the lower ranges.


BLUR
Executes a Guassian blur with the level parameter specifying the extent
of the blurring. If no parameter is used, the blur is equivalent to
Guassian blur of radius 1. Larger values increase the blur.


ERODE
Reduces the light areas. No parameter is used.


DILATE
Increases the light areas. No parameter is used.

**รูปแบบการใช้งาน**

filter ( filterType, filterParam )

**พารามิเตอร์**

- ``filterType``  Constant: either THRESHOLD, GRAY, OPAQUE, INVERT, POSTERIZE, BLUR, ERODE or DILATE

- ``filterParam``  Number: an optional parameter unique to each filter, see above


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var img;
	function preload() {
	  img = loadImage("assets/bricks.jpg");
	}
	function setup() {
	 image(img, 0, 0);
	 filter(THRESHOLD);
	}


	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	var img;
	function preload() {
	  img = loadImage("assets/bricks.jpg");
	}
	function setup() {
	 image(img, 0, 0);
	 filter(GRAY);
	}


	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	var img;
	function preload() {
	  img = loadImage("assets/bricks.jpg");
	}
	function setup() {
	 image(img, 0, 0);
	 filter(OPAQUE);
	}


	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	var img;
	function preload() {
	  img = loadImage("assets/bricks.jpg");
	}
	function setup() {
	 image(img, 0, 0);
	 filter(INVERT);
	}


	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	var img;
	function preload() {
	  img = loadImage("assets/bricks.jpg");
	}
	function setup() {
	 image(img, 0, 0);
	 filter(POSTERIZE,3);
	}


	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	var img;
	function preload() {
	  img = loadImage("assets/bricks.jpg");
	}
	function setup() {
	 image(img, 0, 0);
	 filter(DILATE);
	}


	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	var img;
	function preload() {
	  img = loadImage("assets/bricks.jpg");
	}
	function setup() {
	 image(img, 0, 0);
	 filter(BLUR,3);
	}


	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	var img;
	function preload() {
	  img = loadImage("assets/bricks.jpg");
	}
	function setup() {
	 image(img, 0, 0);
	 filter(ERODE);
	}


	</script>

	<br><br>

.. toctree::

