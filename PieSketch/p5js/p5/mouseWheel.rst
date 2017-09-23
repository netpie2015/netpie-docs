.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mouseWheel()
============

The function mouseWheel() is executed every time a vertical mouse wheel
event is detected either triggered by an actual mouse wheel or by a
touchpad.

The event.delta property returns the amount the mouse wheel
have scrolled. The values can be positive or negative depending on the
scroll direction (on OS X with "natural" scrolling enabled, the signs
are inverted).

Browsers may have different default behaviors attached to various
mouse events. To prevent any default behavior for this event, add
"return false" to the end of the method.

Due to the current support of the "wheel" event on Safari, the function
may only work as expected if "return false" is included while using Safari.

**รูปแบบการใช้งาน**

mouseWheel ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var pos = 25;
	
	function draw() {
	  background(237, 34, 93);
	  fill(0);
	  rect(25, pos, 50, 50);
	}
	
	function mouseWheel(event) {
	  print(event.delta);
	  //move the square according to the vertical scroll amount
	  pos += event.delta;
	  //uncomment to block page scrolling
	  //return false;
	}
	</script>

	<br><br>

.. toctree::

