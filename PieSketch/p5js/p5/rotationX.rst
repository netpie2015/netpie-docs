.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

rotationX
===========

The system variable rotationX always contains the rotation of the
device along the x axis. Value is represented as 0 to +/-180 degrees.

Note: The order the rotations are called is important, ie. if used
together, it must be called in the order Z-X-Y or there might be
unexpected behaviour.

**รูปแบบการใช้งาน**

rotationX

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup(){
	  createCanvas(100, 100, WEBGL);
	}
	
	function draw(){
	  background(200);
	  //rotateZ(radians(rotationZ));
	  rotateX(radians(rotationX));
	  //rotateY(radians(rotationY));
	  box(200, 200, 200);
	}

	</script>

	<br><br>

.. toctree::

