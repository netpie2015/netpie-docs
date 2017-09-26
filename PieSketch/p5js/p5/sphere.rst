.. raw:: html

	<script src="https://sketch.netpie.io/widget/p5-widget.js"></script>

sphere()
========

วาดทรงกลมที่มีรัศมีให้

.. Draw a sphere with given radius
**รูปแบบการใช้งาน**

sphere ( radius, [detailX], [detailY] )

**พารามิเตอร์**

- ``radius``  Number: รัศมีวงกลม

- ``detailX``  Number: ไม่จำเป็น: จำนวนกลุ่มส่วนที่มากขึ้นค่าเริ่มต้นของเรขาคณิตที่ราบรื่นคือ 24

- ``detailY``  Number: ไม่จำเป็น: จำนวนกลุ่มส่วนที่มากขึ้นค่าเริ่มต้นของเรขาคณิตที่ราบรื่นคือ 16

.. ``radius``  Number: radius of circle
.. ``detailX``  Number: optional: number of segments,
                                   the more segments the smoother geometry
                                   default is 24
.. ``detailY``  Number: optional: number of segments,
                                   the more segments the smoother geometry
                                   default is 16

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

.. note:: This document was generated from p5js files whose source code is available on `github <https://github.com/processing/p5.js>`_.
