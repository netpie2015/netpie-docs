.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

cursor()
========

Sets the cursor to a predefined symbol or an image, or makes it visible
if already hidden. If you are trying to set an image as the cursor, the
recommended size is 16x16 or 32x32 pixels. It is not possible to load an
image as the cursor if you are exporting your program for the Web, and not
all MODES work with all browsers. The values for parameters x and y must
be less than the dimensions of the image.

**รูปแบบการใช้งาน**

cursor ( type, [x], [y] )

**พารามิเตอร์**

- ``type``  : either ARROW, CROSS, HAND, MOVE, TEXT, or WAIT, or path for image

- ``x``  : the horizontal active spot of the cursor

- ``y``  : the vertical active spot of the cursor


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Move the mouse left and right across the image
	// to see the cursor change from a cross to a hand
	function draw() {
	  line(width/2, 0, width/2, height);
	  if (mouseX < 50) {
	    cursor(CROSS);
	  } else {
	    cursor(HAND);
	  }
	}
	</script>

	<br><br>

.. toctree::

