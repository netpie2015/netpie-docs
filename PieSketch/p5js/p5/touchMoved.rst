.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

touchMoved()
============

The touchMoved() function is called every time a touch move is registered.
If no touchMoved() function is defined, the mouseDragged() function will
be called instead if it is defined.

Browsers may have different default behaviors attached to various touch
events. To prevent any default behavior for this event, add "return false"
to the end of the method.

**รูปแบบการใช้งาน**

touchMoved ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Move your finger across the page
	// to change its value
	
	var value = 0;
	function draw() {
	  fill(value);
	  rect(25, 25, 50, 50);
	}
	function touchMoved() {
	  value = value + 5;
	  if (value > 255) {
	    value = 0;
	  }
	}


	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	function touchMoved() {
	  ellipse(mouseX, mouseY, 5, 5);
	  // prevent default
	  return false;
	}


	</script>

	<br><br>

.. toctree::

