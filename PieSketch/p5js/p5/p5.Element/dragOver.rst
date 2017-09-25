.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

dragOver()
==========

The .dragOver() function is called once after every time a
file is dragged over the element. This can be used to attach an
element specific event listener.

**รูปแบบการใช้งาน**

dragOver ( fxn )

**พารามิเตอร์**

- ``fxn``  function: function to be fired when mouse is dragged over the element.


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// To test this sketch, simply drag a
	// file over the canvas
	function setup() {
	  var c = createCanvas(100, 100);
	  background(200);
	  textAlign(CENTER);
	  text('Drag file', width/2, height/2);
	  c.dragOver(dragOverCallback);
	}
	
	// This function will be called whenever
	// a file is dragged over the canvas
	function dragOverCallback() {
	  background(240);
	  text('Dragged over', width/2, height/2);
	}

	</script>

	<br><br>

.. toctree::

