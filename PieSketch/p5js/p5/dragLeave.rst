.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

dragLeave()
===========

The .dragLeave() function is called once after every time a
dragged file leaves the element area. This can be used to attach an
element specific event listener.

**รูปแบบการใช้งาน**

dragLeave ( fxn )

**พารามิเตอร์**

- ``fxn``  : function to be fired when mouse is dragged over the element.


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// To test this sketch, simply drag a file
	// over and then out of the canvas area
	function setup() {
	  var c = createCanvas(100, 100);
	  background(200);
	  textAlign(CENTER);
	  text('Drag file', width/2, height/2);
	  c.dragLeave(dragLeaveCallback);
	}
	
	// This function will be called whenever
	// a file is dragged out of the canvas
	function dragLeaveCallback() {
	  background(240);
	  text('Dragged off', width/2, height/2);
	}
	</script>

	<br><br>

.. toctree::

