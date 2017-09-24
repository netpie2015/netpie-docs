.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

touchStarted()
==============

The touchStarted() function is called once after every time a touch is
registered. If no touchStarted() function is defined, the mousePressed()
function will be called instead if it is defined.

Browsers may have different default behaviors attached to various touch
events. To prevent any default behavior for this event, add "return false"
to the end of the method.

**รูปแบบการใช้งาน**

touchStarted ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Touch within the image to change
	// the value of the rectangle
	
	var value = 0;
	function draw() {
	  fill(value);
	  rect(25, 25, 50, 50);
	}
	function touchStarted() {
	  if (value == 0) {
	    value = 255;
	  } else {
	    value = 0;
	  }
	}


	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	function touchStarted() {
	  ellipse(mouseX, mouseY, 5, 5);
	  // prevent default
	  return false;
	}


	</script>

	<br><br>

.. toctree::

