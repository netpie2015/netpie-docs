.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

touchMoved()
============

The .touchMoved() function is called once after every time a touch move is
registered. This can be used to attach element specific event listeners.

**รูปแบบการใช้งาน**

touchMoved ( fxn )

**พารามิเตอร์**

- ``fxn``  function: function to be fired when touch is moved over the element.


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var cnv;
	var g;
	function setup() {
	  cnv = createCanvas(100, 100);
	  cnv.touchMoved(changeGray); // attach listener for
	                              // canvas click only
	  g = 100;
	}
	
	function draw() {
	  background(g);
	}
	
	// this function fires only when cnv is clicked
	function changeGray() {
	  g = random(0, 255);
	}

	</script>

	<br><br>

.. toctree::

