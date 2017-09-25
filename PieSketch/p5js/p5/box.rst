.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

box()
=====

Draw a box with given width, height and depth

**รูปแบบการใช้งาน**

box ( width, [Height], [depth], [detailX], [detailY] )

**พารามิเตอร์**

- ``width``  Number: width of the box

- ``Height``  Number: height of the box

- ``depth``  Number: depth of the box

- ``detailX``  Number: Optional number of triangle subdivisions in x-dimension

- ``detailY``  Number: Optional number of triangle subdivisions in y-dimension


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	//draw a spinning box with width, height and depth 200
	function setup(){
	  createCanvas(100, 100, WEBGL);
	}
	
	function draw(){
	  background(200);
	  rotateX(frameCount * 0.01);
	  rotateY(frameCount * 0.01);
	  box(200, 200, 200);
	}

	</script>

	<br><br>

.. toctree::

