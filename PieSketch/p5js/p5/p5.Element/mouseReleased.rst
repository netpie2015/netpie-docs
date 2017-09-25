.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mouseReleased()
===============

The .mouseReleased() function is called once after every time a
mouse button is released over the element. This can be used to
attach element specific event listeners.

**รูปแบบการใช้งาน**

mouseReleased ( fxn )

**พารามิเตอร์**

- ``fxn``  function: function to be fired when mouse is released over the element.


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var cnv;
	var d;
	var g;
	function setup() {
	  cnv = createCanvas(100, 100);
	  cnv.mouseReleased(changeGray); // attach listener for
	                                 // activity on canvas only
	  d = 10;
	  g = 100;
	}
	
	function draw() {
	  background(g);
	  ellipse(width/2, height/2, d, d);
	}
	
	// this function fires after the mouse has been
	// released
	function mouseReleased() {
	  d = d + 10;
	}
	
	// this function fires after the mouse has been
	// released while on canvas
	function changeGray() {
	  g = random(0, 255);
	}

	</script>

	<br><br>

.. toctree::

