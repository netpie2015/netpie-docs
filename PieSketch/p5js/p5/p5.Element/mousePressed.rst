.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mousePressed()
==============

The .mousePressed() function is called once after every time a
mouse button is pressed over the element. This can be used to
attach element specific event listeners.

**รูปแบบการใช้งาน**

mousePressed ( fxn )

**พารามิเตอร์**

- ``fxn``  function: function to be fired when mouse is pressed over the element.


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var cnv;
	var d;
	var g;
	function setup() {
	  cnv = createCanvas(100, 100);
	  cnv.mousePressed(changeGray); // attach listener for
	                                // canvas click only
	  d = 10;
	  g = 100;
	}
	
	function draw() {
	  background(g);
	  ellipse(width/2, height/2, d, d);
	}
	
	// this function fires with any click anywhere
	function mousePressed() {
	  d = d + 10;
	}
	
	// this function fires only when cnv is clicked
	function changeGray() {
	  g = random(0, 255);
	}

	</script>

	<br><br>

.. toctree::

