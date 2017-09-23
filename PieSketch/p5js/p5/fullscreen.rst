.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

fullscreen()
============

If argument is given, sets the sketch to fullscreen or not based on the
value of the argument. If no argument is given, returns the current
fullscreen state. Note that due to browser restrictions this can only
be called on user input, for example, on mouse press like the example
below.

**รูปแบบการใช้งาน**

fullscreen ( [val] )

**พารามิเตอร์**

- ``val``  : whether the sketch should be in fullscreen mode or not


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// Clicking in the box toggles fullscreen on and off.
	function setup() {
	  background(200);
	}
	function mousePressed() {
	  if (mouseX > 0 && mouseX < 100 && mouseY > 0 && mouseY < 100) {
	    var fs = fullscreen();
	    fullscreen(!fs);
	  }
	}
	</script>

	<br><br>

.. toctree::

