.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

sphere()
========

Draw a sphere with given radius

**รูปแบบการใช้งาน**

sphere ( radius, [detailX], [detailY] )

**พารามิเตอร์**

- ``radius``  : radius of circle

- ``detailX``  : optional: number of segments, the more segments the smoother geometry default is 24

- ``detailY``  : optional: number of segments, the more segments the smoother geometry default is 16


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	// draw a sphere with radius 200
	function setup(){
	  createCanvas(100, 100, WEBGL);
	}
	
	function draw(){
	  background(200);
	  sphere(50);
	}
	</script>

	<br><br>

.. toctree::

