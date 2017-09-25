.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

deviceMoved()
=============

The deviceMoved() function is called when the device is moved by more than
the threshold value along X, Y or Z axis. The default threshold is set to
0.5.

**รูปแบบการใช้งาน**

deviceMoved ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Run this example on a mobile device
	// Move the device around
	// to change the value.
	
	var value = 0;
	function draw() {
	  fill(value);
	  rect(25, 25, 50, 50);
	}
	function deviceMoved() {
	  value = value + 5;
	  if (value > 255) {
	    value = 0;
	  }
	}

	</script>

	<br><br>

.. toctree::

