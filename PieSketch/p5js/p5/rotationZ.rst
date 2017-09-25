.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

rotationZ
===========

The system variable rotationZ always contains the rotation of the
device along the z axis. Value is represented as 0 to 359 degrees.

Unlike rotationX and rotationY, this variable is available for devices
with a built-in compass only.

Note: The order the rotations are called is important, ie. if used
together, it must be called in the order Z-X-Y or there might be
unexpected behaviour.

**รูปแบบการใช้งาน**

rotationZ

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup(){
	  createCanvas(100, 100, WEBGL);
	}
	
	function draw(){
	  background(200);
	  rotateZ(radians(rotationZ));
	  //rotateX(radians(rotationX));
	  //rotateY(radians(rotationY));
	  box(200, 200, 200);
	}

	</script>

	<br><br>

.. toctree::

