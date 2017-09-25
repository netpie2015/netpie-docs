.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mouseClicked()
==============

The mouseClicked() function is called once after a mouse button has been
pressed and then released.

Browsers handle clicks differently, so this function is only guaranteed to be
run when the left mouse button is clicked. To handle other mouse buttons
being pressed or released, see mousePressed() or mouseReleased().

Browsers may have different default
behaviors attached to various mouse events. To prevent any default
behavior for this event, add "return false" to the end of the method.

**รูปแบบการใช้งาน**

mouseClicked ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Click within the image to change
	// the value of the rectangle
	// after the mouse has been clicked
	
	var value = 0;
	function draw() {
	  fill(value);
	  rect(25, 25, 50, 50);
	}
	
	function mouseClicked() {
	  if (value == 0) {
	    value = 255;
	  } else {
	    value = 0;
	  }
	}

	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	function mouseClicked() {
	  ellipse(mouseX, mouseY, 5, 5);
	  // prevent default
	  return false;
	}

	</script>

	<br><br>

.. toctree::

