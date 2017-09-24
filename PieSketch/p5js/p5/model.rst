.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

model()
=======

Render a 3d model to the screen.

**รูปแบบการใช้งาน**

model ( model )

**พารามิเตอร์**

- ``model``  p5.Geometry: Loaded 3d model to be rendered


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	//draw a spinning teapot
	var teapot;
	
	function setup(){
	  createCanvas(100, 100, WEBGL);
	
	  teapot = loadModel('assets/teapot.obj');
	}
	
	function draw(){
	  background(200);
	  rotateX(frameCount * 0.01);
	  rotateY(frameCount * 0.01);
	  model(teapot);
	}


	</script>

	<br><br>

.. toctree::

