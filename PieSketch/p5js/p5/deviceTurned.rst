.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

deviceTurned()
==============

The deviceTurned() function is called when the device rotates by
more than 90 degrees continuously.

The axis that triggers the deviceTurned() method is stored in the turnAxis
variable. The deviceTurned() method can be locked to trigger on any axis:
X, Y or Z by comparing the turnAxis variable to 'X', 'Y' or 'Z'.

**รูปแบบการใช้งาน**

deviceTurned ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Run this example on a mobile device
	// Rotate the device by 90 degrees
	// to change the value.
	
	var value = 0;
	function draw() {
	  fill(value);
	  rect(25, 25, 50, 50);
	}
	function deviceTurned() {
	  if (value == 0){
	    value = 255
	  } else if (value == 255) {
	    value = 0;
	  }
	}
	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Run this example on a mobile device
	// Rotate the device by 90 degrees in the
	// X-axis to change the value.
	
	var value = 0;
	function draw() {
	  fill(value);
	  rect(25, 25, 50, 50);
	}
	function deviceTurned() {
	  if (turnAxis == 'X'){
	    if (value == 0){
	      value = 255
	    } else if (value == 255) {
	      value = 0;
	    }
	  }
	}
	</script>

	<br><br>

.. toctree::

