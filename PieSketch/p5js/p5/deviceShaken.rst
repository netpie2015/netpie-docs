.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

deviceShaken()
==============

The deviceShaken() function is called when the device total acceleration
changes of accelerationX and accelerationY values is more than
the threshold value. The default threshold is set to 30.

**รูปแบบการใช้งาน**

deviceShaken ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Run this example on a mobile device
	// Shake the device to change the value.
	
	var value = 0;
	function draw() {
	  fill(value);
	  rect(25, 25, 50, 50);
	}
	function deviceShaken() {
	  value = value + 5;
	  if (value > 255) {
	    value = 0;
	  }
	}

	</script>

	<br><br>

.. toctree::

