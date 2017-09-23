.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

doubleClicked()
===============

The doubleClicked() function is executed every time a event
listener has detected a dblclick event which is a part of the
DOM L3 specification. The doubleClicked event is fired when a
pointing device button (usually a mouse's primary button)
is clicked twice on a single element. For more info on the
dblclick event refer to mozilla's documentation here:
https://developer.mozilla.org/en-US/docs/Web/Events/dblclick

**รูปแบบการใช้งาน**

doubleClicked ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Click within the image to change
	// the value of the rectangle
	// after the mouse has been double clicked
	
	var value = 0;
	function draw() {
	  fill(value);
	  rect(25, 25, 50, 50);
	}
	
	function doubleClicked() {
	  if (value == 0) {
	    value = 255;
	  } else {
	    value = 0;
	  }
	}
	</script>

	<br><br>

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	
	function doubleClicked() {
	  ellipse(mouseX, mouseY, 5, 5);
	  // prevent default
	  return false;
	}
	</script>

	<br><br>

.. toctree::

