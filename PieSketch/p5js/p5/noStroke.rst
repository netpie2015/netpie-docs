.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

noStroke()
==========

Does not render stroke

**รูปแบบการใช้งาน**

noStroke ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup(){
	  createCanvas(200, 200, WEBGL);
	}
	
	function draw(){
	 background(0);
	 noStroke();
	 fill(240, 150, 150);
	 rotateX(frameCount * 0.01);
	 rotateY(frameCount * 0.01);
	 box(75, 75, 75);
	}
	</script>

	<br><br>

.. toctree::

