.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

strokeWeight()
==============

Change weight of stroke

**รูปแบบการใช้งาน**

strokeWeight ( stroke )

**พารามิเตอร์**

- ``stroke``  : weight to be used for drawing


.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup(){
	  createCanvas(200, 400, WEBGL);
	  setAttributes('antialias', true);
	}
	
	function draw(){
	  background(0);
	  noStroke();
	  translate(0,-100,0);
	  stroke(240,150,150);
	  fill(100,100,240);
	  push();
	  strokeWeight(8);
	  rotateX(frameCount * 0.01);
	  rotateY(frameCount * 0.01);
	  sphere(75);
	  pop();
	  push();
	  translate(0,200,0);
	  strokeWeight(1);
	  rotateX(frameCount * 0.01);
	  rotateY(frameCount * 0.01);
	  sphere(75);
	  pop();
	}
	
	</script>

	<br><br>

.. toctree::

