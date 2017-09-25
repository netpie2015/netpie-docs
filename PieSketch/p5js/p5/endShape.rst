.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

endShape()
==========

The endShape() function is the companion to beginShape() and may only be
called after beginShape(). When endshape() is called, all of image data
defined since the previous call to beginShape() is written into the image
buffer. The constant CLOSE as the value for the MODE parameter to close
the shape (to connect the beginning and the end).

**รูปแบบการใช้งาน**

endShape ( [mode] )

**พารามิเตอร์**

- ``mode``  Constant: use CLOSE to close the shape


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	noFill();
	
	beginShape();
	vertex(20, 20);
	vertex(45, 20);
	vertex(45, 80);
	endShape(CLOSE);
	
	beginShape();
	vertex(50, 20);
	vertex(75, 20);
	vertex(75, 80);
	endShape();

	</script>

	<br><br>

.. toctree::

