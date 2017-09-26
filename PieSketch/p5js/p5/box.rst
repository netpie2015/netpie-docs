.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

box()
=====

วาดช่องที่มีความกว้างความสูงและความลึก

.. Draw a box with given width, height and depth
**รูปแบบการใช้งาน**

box ( width, [Height], [depth], [detailX], [detailY] )

**พารามิเตอร์**

- ``width``  Number: ความกว้างของกล่อง

- ``Height``  Number: ความสูงของกล่อง

- ``depth``  Number: ความลึกของกล่อง

- ``detailX``  Number: จำนวนตัวเลือกของสามเหลี่ยมใน x-dimension

- ``detailY``  Number: จำนวนตัวอยางของสวนยอยสามเหลี่ยมใน y-dimension

.. ``width``  Number: width of the box
.. ``Height``  Number: height of the box
.. ``depth``  Number: depth of the box
.. ``detailX``  Number: Optional number of triangle
                           subdivisions in x-dimension
.. ``detailY``  Number: Optional number of triangle
                           subdivisions in y-dimension

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

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
