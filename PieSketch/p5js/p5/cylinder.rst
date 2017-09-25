.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

cylinder()
==========

Draw a cylinder with given radius and height

**รูปแบบการใช้งาน**

cylinder ( radius, height, [detailX], [detailY] )

**พารามิเตอร์**

- ``radius``  Number: radius of the surface

- ``height``  Number: height of the cylinder

- ``detailX``  Number: optional: number of segments, the more segments the smoother geometry default is 24

- ``detailY``  Number: optional: number of segments in y-dimension, the more segments the smoother geometry default is 16


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	//draw a spinning cylinder with radius 200 and height 200
	function setup(){
	  createCanvas(100, 100, WEBGL);
	}
	
	function draw(){
	  background(200);
	  rotateX(frameCount * 0.01);
	  rotateZ(frameCount * 0.01);
	  cylinder(200, 200);
	}

	</script>

	<br><br>

.. toctree::

