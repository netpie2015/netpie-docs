.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

torus()
=======

Draw a torus with given radius and tube radius

**รูปแบบการใช้งาน**

torus ( radius, tubeRadius, [detailX], [detailY] )

**พารามิเตอร์**

- ``radius``  : radius of the whole ring

- ``tubeRadius``  : radius of the tube

- ``detailX``  : optional: number of segments in x-dimension, the more segments the smoother geometry default is 24

- ``detailY``  : optional: number of segments in y-dimension, the more segments the smoother geometry default is 16


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	//draw a spinning torus with radius 200 and tube radius 60
	function setup(){
	  createCanvas(100, 100, WEBGL);
	}
	
	function draw(){
	  background(200);
	  rotateX(frameCount * 0.01);
	  rotateY(frameCount * 0.01);
	  torus(200, 60);
	}
	</script>

	<br><br>

.. toctree::

