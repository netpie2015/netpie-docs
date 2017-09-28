.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

noFill()
========

ไม่ทำให้การเติมวัสดุ

.. Does not render fill material

**รูปแบบการใช้งาน**

noFill ( )

.. raw:: html

	<script type="text/p5" data-autoplay data-hide-sourcecode>
	function setup(){
	  createCanvas(200, 200, WEBGL);
	}
	
	function draw(){
	 background(0);
	 noFill();
	 stroke(100, 100, 240);
	 rotateX(frameCount * 0.01);
	 rotateY(frameCount * 0.01);
	 box(75, 75, 75);
	}

	</script>

	<br><br>

..  [#f1] This document was generated from p5.js whose source code is available on `github <https://github.com/processing/p5.js>`_.
