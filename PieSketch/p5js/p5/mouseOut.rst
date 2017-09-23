.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

mouseOut()
==========

The .mouseOut() function is called once after every time a
mouse moves off the element. This can be used to attach an
element specific event listener.

**รูปแบบการใช้งาน**

mouseOut ( fxn )

**พารามิเตอร์**

- ``fxn``  : function to be fired when mouse is moved off the element.


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	var cnv;
	var d;
	var g;
	function setup() {
	  cnv = createCanvas(100, 100);
	  cnv.mouseOut(changeGray);
	  d = 10;
	}
	
	function draw() {
	  ellipse(width/2, height/2, d, d);
	}
	
	function changeGray() {
	  d = d + 10;
	  if (d > 100) {
	    d = 0;
	  }
	}
	</script>

	<br><br>

.. toctree::

