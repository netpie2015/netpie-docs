.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

plane()
=======

Draw a plane with given a width and height

**รูปแบบการใช้งาน**

plane ( width, height, [detailX], [detailY] )

**พารามิเตอร์**

- ``width``  : width of the plane

- ``height``  : height of the plane

- ``detailX``  : Optional number of triangle subdivisions in x-dimension

- ``detailY``  : Optional number of triangle subdivisions in y-dimension


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	//draw a plane with width 200 and height 200
	function setup(){
	  createCanvas(100, 100, WEBGL);
	}
	
	function draw(){
	  background(200);
	  plane(50, 50);
	}
	</script>

	<br><br>

.. toctree::

